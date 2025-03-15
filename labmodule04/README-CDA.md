# Constrained Device Application (Connected Devices)

## Lab Module 04

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
My implementation focuses on creating emulated sensor modules for the SenseHAT in the CDA application. These modules, derived from BaseSensorSimTask, simulate the behavior of the actual SenseHAT sensors using the I2C protocol. I implemented three sensor emulators: HumidityI2cSensorAdapterTask, PressureI2cSensorAdapterTask, and TemperatureI2cSensorAdapterTask. Each module reads data from the I2C bus and returns simulated telemetry data. The goal is to make the CDA read and process data as if it were interacting with physical sensors. I use the smbus library for communication with the I2C bus on the Raspberry Pi, and the sensor addresses are based on the SenseHAT specifications (HTS221, LPS25H).

How does your implementation work?
The implementation works by initializing the I2C bus and the sensor addresses in each class. Then, the generateTelemetry method fetches data from the sensor registers, performs the necessary calculations, and updates the sensor data attributes. I modified the SensorAdapterManager to access these sensors based on the configuration. I also added unit and integration tests to ensure everything works properly, like communication with the I2C bus, sensor data calculations, and integration with the SensorAdapterManager.


### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/marinaacastroo/python-components/tree/labmodule03


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- All part01 unit tests
- HumidityI2cSensorAdapterTest
- PressureI2cSensorAdapterTest
- TemperatureI2cSensorAdapterTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- All part01 integration tests
- SenseHatEmulatorQuickTest.py
- EmbeddedSensorAdapterTest.py


EOF.
