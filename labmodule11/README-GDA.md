# Gateway Device Application (Connected Devices)

## Lab Module 11

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación desarrolla la Gateway Device Application (GDA) para gestionar la comunicación y el procesamiento de datos entre dispositivos IoT y servicios cloud. La GDA permite la recolección, procesamiento y envío de datos de sensores y actuadores, así como la recepción de comandos desde la nube. Además, integra mecanismos de configuración y soporte para certificados, facilitando la operación segura y flexible del sistema.

How does your implementation work?
La aplicación está organizada en módulos independientes, cada uno encargado de una función específica: gestión de datos, conectividad MQTT/CoAP, y manejo de eventos de sensores y actuadores. Los datos se procesan localmente y se transmiten a la nube mediante los conectores implementados. El uso de archivos de configuración permite adaptar fácilmente la aplicación a diferentes entornos. Se han incluido pruebas unitarias e integración para asegurar la calidad y estabilidad del sistema, y el diseño modular permite futuras ampliaciones.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/java-components/tree/labmodule11


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- ResourceNameTest
- SystemCpuUtilTaskTest
- SystemMemUtilTaskTest
- ActuatorDataTest
- BaseIotDataTest
- DataUtilTest
- SensorDataTest
- SystemPerformanceDataTest
- SystemStateDataTest
- SimpleCertManagementUtilTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- GatewayDeviceAppTest
- SystemPerformanceManagerTest
- DeviceDataManagerNoCommsTest
- DataIntegrationTest
- PersistenceClientAdapterTest
- DeviceDataManagerSimpleCdaActuationTest
- DeviceDataManagerWithCommsTest
- CoapClientConnectorTest
- CoapClientPerformanceTest
- CoapClientToServerConnectorTest
- CoapServerGatewayTest
- MqttClientConnectorTest
- MqttClientControlPacketTest
- MqttClientPerformanceTest
- MqttPublishDataMessageListener
- CloudClientConnectorTest
- SmtpClientConnectorTest


EOF.
