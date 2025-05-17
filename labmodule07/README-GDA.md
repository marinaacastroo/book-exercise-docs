# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
My implementation adds MQTT support to the GDA, enabling it to publish, subscribe to, and receive messages from an MQTT broker. I implemented the MqttClientConnector class to manage the connection and communication using the synchronous MqttClient. I also configured the necessary topic subscriptions to receive data from the CDA and integrated the connector into the DeviceDataManager.

How does your implementation work?
The MQTT client is initialized with values from the configuration file and started from within the DeviceDataManager. Messages are published and received through methods that validate the topic and QoS level. Connection events, message delivery, and incoming messages are handled using the MqttCallbackExtended interface. To complete the lab, I captured all 14 MQTT 3.1.1 control packets using Wireshark by sending messages with QoS 1 and 2.


### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: 


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- 
- 
- 

EOF.
