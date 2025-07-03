# Constrained Device Application (Connected Devices)

## Lab Module 09

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
My implementation for Lab Module 09 extends the Constrained Device Application (CDA) to support MQTT-based messaging, following the requirements specified in the PIOT-CDA-* issues. The code enables the CDA to connect to an MQTT broker, publish telemetry data, and subscribe to relevant topics for actuator commands. It also ensures that configuration parameters such as host, port, QoS, and client ID are loaded dynamically, and that the MQTT client can be cleanly started and stopped as required.

How does your implementation work?
The implementation uses the Paho MQTT client library to manage MQTT connections and messaging. The MqttClientConnector class is responsible for establishing the connection to the broker, handling callbacks for connect, disconnect, message, publish, and subscribe events, and providing methods to publish and subscribe to topics. Configuration values are loaded using the ConfigUtil class, ensuring flexibility and reusability. The code is structured to allow easy integration with the rest of the CDA system, and all methods are designed to handle errors gracefully and log relevant information for debugging and monitoring.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule09



### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- DataUtilTest
- SensorDataTest
- SystemPerformanceDataTest
- SystemStateDataTest
- BaseDeviceSimulatorTest
- SensorSimAdapterManagerTest
- DeviceDataManagerTest
- CloudClientConnectorTest
- MqttClientConnectorTest
- CoapClientConnectorTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SensorSimAdapterManagerTest
- DeviceDataManagerTest
- CloudClientConnectorTest
- MqttClientConnectorTest
- CoapClientConnectorTest

EOF.
