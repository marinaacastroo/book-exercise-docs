# Gateway Device Application (Connected Devices)

## Lab Module 12 - Semester Project - GDA Components

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi GDA funciona como un puente seguro entre el CDA local (que ahora incorpora un sensor de calidad del aire) y la nube (Ubidots). Recoge datos de sensores del CDA, como temperatura, humedad y calidad del aire, así como métricas de funcionamiento de los dispositivos, y los envía a la nube para su visualización y análisis. Además, si el GDA detecta que la calidad del aire reportada por el CDA es deficiente según los umbrales definidos, envía una orden al CDA para activar un nuevo actuador, como un purificador de aire. El GDA también recibe comandos desde la nube, por ejemplo, para encender un LED, y los retransmite al CDA para su ejecución. Para mantener informado al usuario, el GDA envía notificaciones por correo electrónico cuando se activan actuadores y almacena los datos localmente.

How does your implementation work?
El GDA utiliza MQTT con TLS para garantizar una comunicación segura tanto con el CDA como con la plataforma Ubidots. Un DeviceDataManager centraliza la gestión del flujo de datos: cuando recibe lecturas del sensor de calidad del aire del CDA, las analiza y, si detecta valores por debajo del umbral durante un periodo determinado, genera un comando ActuatorData para el purificador de aire y lo envía al CDA mediante MQTT. Todos los datos de sensores, incluyendo el nuevo sensor de calidad del aire, se envían a la nube a través de CloudClientConnector, que adapta los tópicos al formato requerido por Ubidots. Para los comandos provenientes de la nube (como el control del LED), CloudClientConnector se suscribe a los tópicos de Ubidots y, al recibir una señal, un listener interno la transforma en un ActuatorData que se pasa a DeviceDataManager para su reenvío al CDA. Además, SmtpClientConnector se encarga de enviar notificaciones por correo electrónico cada vez que se activa un actuador.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/java-components/tree/labmodule12



### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- 
- 
- 

EOF.
