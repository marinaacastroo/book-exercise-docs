# Gateway Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? Mi implementación crea e integra un servidor CoAP en el gateway IoT utilizando la librería Eclipse Californium, permitiendo la comunicación eficiente y estandarizada entre dispositivos IoT y el gateway. El servidor CoAP expone recursos clave como el rendimiento del sistema, telemetría y comandos de actuador, cada uno gestionado por su propio handler especializado. Estos handlers procesan las peticiones entrantes (GET, PUT, etc.), actualizan el estado interno y notifican a los listeners correspondientes, permitiendo así la recepción y el procesamiento de datos en tiempo real desde dispositivos remotos. Además, la solución soporta la funcionalidad de descubrimiento de recursos y la observación (OBSERVE) para notificar cambios en los datos de actuador, cumpliendo con los requisitos de interoperabilidad y extensibilidad del laboratorio.

How does your implementation work? El funcionamiento se basa en la inicialización del servidor CoAP dentro de la clase CoapServerGateway, donde se registran los recursos y se asocian a sus handlers. El gateway se integra con la clase DeviceDataManager, que implementa la interfaz de listener para recibir y procesar los datos de los recursos. Al arrancar el servidor, los clientes pueden descubrir los recursos disponibles y realizar operaciones sobre ellos usando clientes CoAP estándar, como el cliente CLI de Californium. Los handlers gestionan las peticiones, convierten los datos recibidos (por ejemplo, en formato JSON) a objetos internos y notifican a los listeners para su procesamiento. El diseño modular permite añadir o modificar recursos fácilmente y asegura que el gateway pueda interactuar con diferentes tipos de dispositivos IoT de manera robusta y escalable.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/java-components/tree/labmodule08


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- All part01
- All part02
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- All part01
- All part02
- CoapServerAdapterTest
- CoapClientToServerConnectorTest

  

EOF.
