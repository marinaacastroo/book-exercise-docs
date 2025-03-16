# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
My implementation focuses on handling data conversion between objects and JSON format for the CDA. This is important because the system needs to serialize and deserialize data efficiently when communicating between different components. The DataUtil module takes care of converting SensorData, ActuatorData, and SystemPerformanceData into JSON and back, making it easier to store, send, and process data.

How does your implementation work?
The way it works is pretty straightforward: it uses Python’s json module along with a custom encoder to handle object serialization. When converting from JSON back to objects, it checks the structure, updates the relevant attributes, and ensures the data matches the expected format. This way, the CDA can easily work with structured data without worrying about manual conversions or errors.


### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule05


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- DataUtilTest
- All part01 unit tests
  

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- All part01 integration tests
  

EOF.
