# Constrained Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación desarrolla la aplicación Constrained Device Application (CDA) para el proyecto de Connected Devices, cumpliendo con todos los requisitos PIOT-CDA-del Lab Module 10. El sistema gestiona la adquisición, procesamiento y transmisión de datos de sensores y actuadores, integrando funcionalidades de configuración, simulación y conectividad (local y remota) mediante protocolos como MQTT y CoAP. Además, implementa la gestión de datos, listeners y adaptadores para sensores y actuadores, permitiendo la emulación y simulación de dispositivos IoT en un entorno controlado.

How does your implementation work?
La arquitectura se basa en una estructura modular, donde cada componente (gestor de datos, conectores, adaptadores de sensores/actuadores, utilidades de configuración) está desacoplado y es fácilmente testeable. El flujo principal inicia con la configuración del sistema, seguido por la inicialización de los adaptadores de sensores y actuadores, y la gestión de los datos a través del DeviceDataManager. Los datos se procesan y se transmiten usando los conectores MQTT y CoAP, permitiendo la interoperabilidad con otros sistemas IoT. La implementación incluye listeners para eventos y telemetría, así como utilidades para la serialización y deserialización de datos, asegurando la robustez y escalabilidad del sistema.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule10


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


### CDA MQTT Client Performance Test Results
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
