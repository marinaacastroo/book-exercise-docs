# Constrained Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
For this lab, I implemented a CoAP server using the aiocoap library within the Constrained Device Application (CDA). The server is set up through the CoapServerAdapter class and supports resource discovery and basic request handling for GET, POST, PUT, and DELETE methods. I also created and registered resource handlers for telemetry, system performance, and actuator updates using ObservableResource subclasses. These resources respond to incoming CoAP requests and will allow future integration with CoAP clients.

How does your implementation work?
The CoapServerAdapter initializes a root resource tree using aiocoap.resource.Site() and registers handlers based on ResourceNameEnum paths. The server runs asynchronously in a separate thread and is started/stopped through the DeviceDataManager. I implemented the required resource handler classes (GetSystemPerformanceResourceHandler, GetTelemetryResourceHandler, and UpdateActuatorResourceHandler), which currently log requests and respond with JSON-formatted mock data. The integration test confirms the server responds correctly to discovery and GET requests, showing all resources are properly registered and accessible.

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
