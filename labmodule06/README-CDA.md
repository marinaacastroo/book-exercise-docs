# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Se establece una conexión con el broker MQTT que gestiona eventos de conexión (CONNECT/CONNACK) y desconexión (DISCONNECT); se configuran callbacks para manejar la recepción de mensajes (onMessage) y notificar eventos de publicación, suscripción y desconexión. Además, se habilitan las funciones de publicación y suscripción mediante la validación de tópicos y QoS, permitiendo enviar y recibir mensajes de manera robusta. También se incorporan pruebas de integración que, ampliadas según sea necesario, generan y validan todos los 14 paquetes de control MQTT, incluyendo el mecanismo de keep‑alive (PINGREQ/PINGRESP) y los flujos para QoS 1 y QoS 2.

How does your implementation work?
Se establece una conexión con el broker MQTT asignando callbacks para gestionar los eventos claves: conexión, desconexión, publicación, suscripción y recepción de mensajes. Al publicar o suscribirse, se validan los tópicos y los niveles de QoS configurados, lo que permite enviar y recibir mensajes de forma robusta y en tiempo real entre los dispositivos. Además, la implementación incorpora pruebas (unitarias e integradas) para verificar que se generan correctamente todos los paquetes de control MQTT, incluyendo el mecanismo de keep‑alive (PINGREQ/PINGRESP) y la secuencia de control para QoS 1 y 2. En conjunto, esto asegura una coordinación efectiva entre la adquisición de datos, su procesamiento y la comunicación con servicios externos mediante MQTT


### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule06


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- all part01 unit test
- all part02 unit test


### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)


- all part01 integration test
- all part02 integration test
- MqttClientConnectorTest
- MqttClientControlPacketTest

EOF.
