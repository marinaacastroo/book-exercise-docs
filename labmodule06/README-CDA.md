# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación del Lab Module 06 se centra en consolidar el trabajo realizado en módulos anteriores y asegurar una integración fluida de todas las funcionalidades clave del CDA. En esta etapa, revisé cuidadosamente los cambios introducidos en la rama labmodule06, los validé mediante pruebas unitarias e integradas de las partes 01, 02 y 03, y finalmente realicé la fusión de la rama con la rama principal del repositorio. Esta integración garantiza que la aplicación esté alineada con la arquitectura propuesta para dispositivos conectados y que todos los componentes trabajen de forma coordinada: adquisición de datos, procesamiento y comunicación con servicios externos mediante MQTT o almacenamiento local.

How does your implementation work?
Primero, revisé los cambios de código en la rama labmodule06 y ejecuté todas las pruebas disponibles utilizando el comando python -m unittest discover para asegurar que no haya errores ni conflictos de integración. Luego, comprobé que los resultados fueran correctos tanto a nivel de unidad como de integración. Tras validar todo, realicé el merge con la rama primary utilizando Git, verifiqué el historial con git log --oneline primary y subí los cambios al repositorio remoto. De este modo, el CDA quedó completamente integrado y preparado para su ejecución como sistema funcional dentro de un entorno IoT.
### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule06


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- SystemCpuUtilTaskTest
- SystemMemUtilTaskTest
- ActuadorDataTest
- BaseIoTDataTest
- DataUtilTest
- SensorDataTest
- SystemPerformanceDataTest
- HumidifierActuatorSimTaskTest
- HumiditySensorSimTaskTest
- HvacActuatorSimTaskTest
- PressureSensorSimTaskTest
- TemperatureSensorSimTaskTest


### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)


- ConstrainedDeviceAppTest
- SystemPerformanceManagerTest
- SensorAdapterManagerTest
- ActuatorAdapterManagerTest
- DeviceDataManagerNoCommsTest
- SenseHatEmulatorQuickTest
- HumidityEmulatorTaskTest
- PressureEmulatorTaskTest
- TemperatureEmulatorTaskTest
- HumidifierEmulatorTaskTest
- HvacEmulatorTaskTest
- LedDisplayEmulatorTaskTest
- SensorEmulatorManagerTest
- ActuatorEmulatorManagerTest
- DataIntegrationTest
- MqttClientConnectorTest

EOF.
