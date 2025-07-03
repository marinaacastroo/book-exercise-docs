# Cloud Service Functions (Connected Devices)

## Lab Module 12 - Semester Project - CSF Components

Be sure to implement all the PIOT-CSF-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi servicio en la nube (Ubidots STEM) actúa como el destino final para los datos generados por mis dispositivos IoT (CDA y GDA). Se conecta de manera segura con el GDA para recibir y almacenar información de sensores como temperatura, humedad, calidad del aire y métricas de funcionamiento de los dispositivos. Toda esta información se visualiza en gráficos dentro de la plataforma Ubidots. Además, he configurado Ubidots para enviar comandos que permiten encender o apagar un LED en el CDA, utilizando un interruptor en el dashboard, lo que demuestra el control remoto desde la nube.

How does your implementation work?
Utilizo la plataforma Ubidots STEM sin necesidad de programar la parte cloud. He creado un dispositivo virtual para el GDA y variables específicas para cada dato que quiero registrar. El GDA envía estos datos mediante MQTT a los tópicos correspondientes de Ubidots (por ejemplo, /v1.6/devices/mi-gda/calidad-aire). Para el control del LED, añadí una variable adicional en Ubidots (comando-led) y la vinculé a un interruptor en el dashboard, permitiendo así el control remoto desde la interfaz web.

### Code Documentation (only applies if you wrote CSF-specific code, otherwise, ignore)

#### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: 


#### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

#### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- 
- 
- 

EOF.
