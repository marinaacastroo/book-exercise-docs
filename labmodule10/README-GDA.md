# Gateway Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación permite que el gateway se conecte a la nube, envíe datos de sensores y rendimiento, y gestione la suscripción a eventos cloud. Para ello, desarrollé la clase CloudClientConnector, que implementa la interfaz ICloudClient y maneja la lógica de conexión, envío y recepción de datos usando los recursos y estructuras del proyecto

How does your implementation work?
El funcionamiento se basa en métodos como connectClient, sendEdgeDataToCloud y subscribeToCloudEvents, que gestionan la comunicación con la nube y la integración con el resto del sistema. Se han añadido logs y validaciones para asegurar la robustez y trazabilidad.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/java-components/tree/labmodule10



### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- MqttClientConnectorTest
- MqttClientPerformanceTest
- ConfigUtilTest
- DataUtilTest
 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- MqttClientConnectorTest
- MqttClientPerformanceTest
- DeviceDataManagerTest
- SensorSimAdapterManagerTest

### GDA MQTT Client Performance Test Results

2025-06-30 15:56:19,371:DeviceDataManagerIntegrationTest:INFO:Testing DeviceDataManager class...
2025-06-30 15:56:19,371:ConfigUtil:INFO:Can't load /Users/marinacastro/Documents/IA/2024-2025/2ºCUATRI/PIC/practicasPIC/python-components/config/PiotConfig.props. Trying default: /Users/marinacastro/Documents/IA/2024-2025/2ºCUATRI/PIC/practicasPIC/python-components/config/PiotConfig.props
2025-06-30 15:56:19,371:ConfigUtil:DEBUG:Config: []
2025-06-30 15:56:19,372:ConfigUtil:INFO:Created instance of ConfigUtil: <programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7fec8421c260>
2025-06-30 15:56:19,372:DeviceDataManager:INFO:Local actuation capabilities enabled
2025-06-30 15:56:19,372:DeviceDataManager:INFO:Starting DeviceDataManager...
2025-06-30 15:56:19,372:DeviceDataManager:INFO:Started DeviceDataManager.
2025-06-30 15:57:19,372:DeviceDataManager:INFO:Stopping DeviceDataManager...
2025-06-30 15:57:19,373:DeviceDataManager:INFO:Stopped DeviceDataManager.

----------------------------------------------------------------------
Ran 1 test in 60.002s

OK

EOF.
