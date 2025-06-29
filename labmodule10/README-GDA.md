# Gateway Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

How does your implementation work?

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




[INFO] Scanning for projects...
[INFO] 
[INFO] --------------< programmingtheiot.gda:gateway-device-app >--------------
[INFO] Building Gateway Device App 0.0.1
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ gateway-device-app ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory /mnt/c/Users/Usuario/OneDrive - Universidade de Vigo/Documentos/IA/PIC/java-components/src/main/resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ gateway-device-app ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ gateway-device-app ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory /mnt/c/Users/Usuario/OneDrive - Universidade de Vigo/Documentos/IA/PIC/java-components/src/test/resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ gateway-device-app ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:3.0.0:test (default-test) @ gateway-device-app ---
[WARNING] useSystemClassLoader setting has no effect when not forking
[WARNING] The parameter forkCount should likely not be 0. Forking a JVM for tests improves test accuracy. Ensure to have a <forkCount> >= 1.  
[INFO] Using auto detected provider org.apache.maven.surefire.junit4.JUnit4Provider
[INFO] Running programmingtheiot.part03.integration.connection.CoapClientPerformanceTest
Jun 30, 2025 12:46:14 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest testPutRequestCon
INFO: Testing PUT - CON
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
Jun 30, 2025 12:46:34 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest execTestPut
INFO: PUT message - useCON = true [10000]: 18891 ms
Jun 30, 2025 12:46:34 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest testPutRequestNon
INFO: Testing PUT - NON
Jun 30, 2025 12:46:56 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest execTestPut
INFO: PUT message - useCON = false [10000]: 22122 ms
Jun 30, 2025 12:46:56 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest testPostRequestCon
INFO: Testing POST - CON
Jun 30, 2025 12:47:13 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest execTestPost
INFO: POST message - useCON = true [10000]: 16977 ms
Jun 30, 2025 12:47:13 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest testPostRequestNon
INFO: Testing POST - NON
Jun 30, 2025 12:47:30 AM programmingtheiot.part03.integration.connection.CoapClientPerformanceTest execTestPost
INFO: POST message - useCON = false [10000]: 17506 ms
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 76.481 s - in programmingtheiot.part03.integration.connection.CoapClientPerformanceTest
[INFO]
[INFO] Results:
[INFO]
[INFO] Tests run: 4, Failures: 0, Errors: 0, Skipped: 0
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:21 min
[INFO] Finished at: 2025-06-30T00:47:30+02:00
[INFO] ------------------------------------------------------------------------

EOF.
