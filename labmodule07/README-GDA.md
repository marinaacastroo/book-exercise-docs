# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación integra el cliente MQTT en DeviceDataManager, permitiendo que el sistema establezca una conexión con un broker MQTT, se suscriba a los tópicos necesarios y gestione el envío y recepción de mensajes. Esto facilita la coordinación entre dispositivos y el intercambio de datos de forma eficiente.


How does your implementation work?
Mi implementación funciona de la siguiente manera: durante la inicialización del DeviceDataManager se evalúa la bandera enableMqttClient para decidir si se debe crear una instancia del cliente MQTT (MqttClientConnector); en caso afirmativo, se configura el cliente con los parámetros del broker obtenidos de la configuración (host, puerto, keep-alive, etc.) y, al arrancar el manager mediante startManager(), se invoca el método connectClient() para establecer conexión y suscribirse a los tópicos necesarios para la comunicación. Durante el funcionamiento, el cliente se encarga de gestionar el envío y la recepción de mensajes, invocando los callbacks correspondientes para confirmar la entrega o procesar la llegada de mensajes, y al detener el sistema con stopManager() se realizan las desuscripciones y se cierra la conexión a través del método disconnectClient().

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/java-components/tree/labmodule07


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- All part 01 unit test
- All part 02 unit test
  
### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- All part01 integration test
- All part02 integration test
- MqttClientConnectorTest
- MqttClientControlPacketTest

EOF.
