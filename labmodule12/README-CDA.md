# Constrained Device Application (Connected Devices)

## Lab Module 12 - Semester Project - CDA Components

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
My implementation for Lab Module 12 focuses on fulfilling all the PIOT-CDA-* requirements for the Constrained Device Application (CDA) components. The solution integrates the necessary modules to enable device connectivity, data acquisition, processing, and communication with cloud and local services. The design follows a modular approach, ensuring that each component—such as configuration management, data handling, and device simulation—can be developed, tested, and maintained independently. Special attention was given to code readability, extensibility, and adherence to best practices, including the use of interfaces and dependency injection where appropriate.

How does your implementation work?
The implementation works by orchestrating the interaction between simulated sensors, actuators, and the core application logic. Data from sensors is collected, processed, and, depending on configuration, sent to cloud endpoints or local consumers. The application leverages configuration files for flexible deployment and supports both unit and integration testing to ensure reliability. All PIOT-CDA-* issues were addressed, and the codebase was kept compatible with previous modules to avoid regressions.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule12


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- All

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- All

EOF.
