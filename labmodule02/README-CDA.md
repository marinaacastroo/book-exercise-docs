# Constrained Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
In this implementation I added system performance monitoring to collect CPU and memory usage data. The CDA uses a SystemPerformanceManager to handle the data collection tasks. These tasks, SystemCpuUtilTask and SystemMemUtilTask, run periodically to gather the system's CPU and memory usage stats, and then log them using the system logger.

How does your implementation work?
The CDA implementation works by setting up a task scheduler within the SystemPerformanceManager module. This manager is responsible for periodically triggering the collection of system performance metrics. The SystemCpuUtilTask gathers CPU utilization data, while the SystemMemUtilTask collects memory usage metrics. These tasks are integrated into the SystemPerformanceManager, allowing the system to start and stop data collection dynamically. The tasks execute at predefined intervals, and the collected data is logged in real-time. This approach provides a simple yet efficient mechanism for monitoring the performance of constrained devices. 

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule02

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- SystemCpuUtilTaskTest
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- ConstrainedDeviceAppTest
- SystemPerformanceManagerTest
- SystemMemUtilTaskTest


EOF.
