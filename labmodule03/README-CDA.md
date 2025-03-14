# Constrained Device Application (Connected Devices)

## Lab Module 03

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
In this implementation, the ConstrainedDeviceApp has been updated to integrate the DeviceDataManager. This was accomplished by creating an instance of DeviceDataManager within the ConstrainedDeviceApp constructor and ensuring that the manager's startManager() and stopManager() methods are invoked appropriately within the app's startApp() and stopApp() methods. Furthermore, all references to the SystemPerformanceManager were removed, as instructed in PIOT-CDA-03-009. The DeviceDataManager was also enhanced to ensure proper communication between SystemPerformanceManager, SensorAdapterManager, and ActuatorAdapterManager, setting up callbacks to pass messages between components.

How does your implementation work?
This solution allows the ConstrainedDeviceApp to handle data from sensors and actuators seamlessly while managing the app's startup and shutdown operations. The system is now fully equipped to start and stop the data manager as part of the device's lifecycle, handling sensor and actuator operations efficiently without the previously used system performance management. The DeviceDataManager now manages these components directly, streamlining the app's functionality.


### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule03

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ActuatorDataTest
- SensorDataTest
- SystemPerformanceDataTest
- HumidifierActuatorSimTaskTest
- HvacActuatorSimTaskTest
- All unit tests in ./src/test/python/programmingtheiot/part02/unit
- All part01 unit tests

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SensorAdapterManagerTest
- ConstrainedDeviceAppTest
- DeviceDataManagerNoCommsTest
- ActuatorAdapterManagerTest
- All part01 integration tests 

EOF.
