# Gateway Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
In my implementation, I focused on the integration between the Gateway Device Application (GDA) and the connected devices (CDA). The core function of the GDA is to collect sensor data from the devices, process the data as needed, and ensure it is serialized in a format suitable for further use, such as JSON, which is then transmitted over the network. Additionally, the GDA handles converting the received data from the CDA into readable, standardized formats for easier manipulation and analysis. This process includes managing multiple devices by listening to their data streams and making sure the data is stored or transmitted as per the system's requirements. The system allows communication between various IoT devices, ensuring real-time updates are available while maintaining synchronization with the cloud infrastructure.

How does your implementation work?
My implementation works by first initializing a communication bridge between the GDA and CDA. It uses Python for the CDA to handle sensor data generation and management, while the GDA uses Java to manage data processing, serialization, and interaction with a cloud service or database. The data is first captured by the CDA using the emulated sensors (like the SenseHAT), then it’s formatted into JSON objects and passed to the GDA. Once the GDA receives the data, it parses the JSON, processes it as necessary (e.g., checking for anomalies, adding metadata), and stores or forwards it to a database or cloud endpoint. Throughout the implementation, the data flow is carefully managed to ensure that sensor data is updated and retrieved in a synchronized manner, with all edge cases handled by appropriate error handling mechanisms.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: 


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- DataUtilTest
- SensorDataProcessingTest
- DeviceConnectionTest
- CloudIntegrationTest 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SensorSimAdapterManagerTest
- DeviceDataManagerTest
- CloudDataSyncTest
- DataStorageTest
- GatewayDeviceCommunicationTest

EOF.
