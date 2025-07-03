# Cloud Service Functions (Connected Devices)

## Lab Module 11

These optional components may be included in your assignment, but are not required. If you choose to implement them, be sure to complete this README and review all the PIOT-CSF-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Mi implementación amplía la Gateway Device Application para soportar funciones cloud básicas para dispositivos conectados. Permite la comunicación entre dispositivos IoT y plataformas cloud principalmente usando los protocolos MQTT y CoAP. El sistema gestiona datos de sensores y actuadores, y facilita la integración con servicios cloud para el envío y recepción de mensajes. Además, incluye mecanismos de configuración y soporte para certificados, así como manejo básico de errores para asegurar operaciones estables.

How does your implementation work?
La solución está estructurada en componentes modulares, cada uno encargado de un aspecto concreto de la conectividad cloud. Los datos de los dispositivos se procesan localmente y se transmiten a la nube mediante el conector adecuado (MQTT o CoAP). La aplicación utiliza archivos de configuración para facilitar el despliegue flexible y cuenta con pruebas unitarias e integración para validar la funcionalidad y evitar regresiones. El código está organizado para permitir futuras extensiones e integración con otros servicios cloud si se requiere.

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
