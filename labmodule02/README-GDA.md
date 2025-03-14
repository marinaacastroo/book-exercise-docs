# Gateway Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-GDA-* issues.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
My implementation integrates system performance monitoring into the Gateway Device Application by connecting SystemCpuUtilTask and SystemMemUtilTask to the SystemPerformanceManager. This allows the system to periodically collect and log CPU and memory utilization metrics, helping with performance monitoring and debugging. The scheduled execution of telemetry retrieval ensures that up-to-date performance data is always available.

How does your implementation work?
The implementation works by utilizing a scheduled executor service within SystemPerformanceManager, which runs the handleTelemetry() method at fixed intervals. This method retrieves telemetry values from SystemCpuUtilTask and SystemMemUtilTask and logs them for further analysis. The startManager() method initializes this process, while stopManager() ensures a graceful shutdown of the scheduled task. The integration was verified through unit and integration tests to confirm correct functionality.
### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/java-components/tree/labmodule02


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- SystemCpuUtilTaskTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- GatewayDeviceAppTest
- 

EOF.
