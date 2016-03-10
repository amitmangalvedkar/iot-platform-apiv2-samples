Device Management Samples
============================================

Following stand-alone samples(present in this project) interacts with IBM Watson IoT Platform using the platform API Version 2 to demonstrate various capabilities of the API.

* [SampleBulkAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleBulkAPIOperations.java) - Sample that showcases how to get, add or remove devices in bulk from Internet of Things Foundation.
* [SampleDeviceTypeAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleDeviceTypeAPIOperations.java) - Sample that showcases various Device Type API operations like list all, create, delete, view and update device types in Internet of Things Foundation.
* [SampleDeviceAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleDeviceAPIOperations.java) - A sample that showcases various Device operations like list, add, remove, view, update, view location and view management information of a device in Internet of Things Foundation.
* [SampleDeviceDiagnosticsAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleDeviceDiagnosticsAPIOperations.java) - A sample that showcases various Device Diagnostic operations like clear logs, retrieve logs, add log information, delete logs, get specific log, clear error codes, get device error codes and add an error code to Internet of Things Foundation.
* [SampleHistorianAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleHistorianAPIOperations.java) - A sample that showcases how to retrieve historical events from Internet of Things Foundation.
* [SampleDeviceManagementAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleDeviceManagementAPIOperations.java) - A sample that showcases various device management request operations that can be performed on Internet of Things Foundation.
* [SampleUsageManagementAPIOperations](https://github.com/ibm-messaging/iot-platform-apiv2-samples/tree/master/java/api-samples-v2/src/main/java/com/ibm/iotf/sample/client/application/api/SampleUsageManagementAPIOperations.java) - A sample that showcases various Usage management operations that can be performed on Internet of Things Foundation..

The samples are written using the [Java Client Library](https://github.com/ibm-messaging/iot-java) for IBM Watson IoT Platform that simplifies the interactions with the IBM Watson IoT Platform.

----

### Prerequisites
To build and run the sample, you must have the following installed:

* [git](https://git-scm.com/)
* [maven](https://maven.apache.org/download.cgi)
* Java 7+

----

### Register Device in IBM Watson IoT Platform

Follow the steps in [this recipe](https://developer.ibm.com/recipes/tutorials/how-to-register-devices-in-ibm-iot-foundation/) to register your device in Watson IoT Platform if not registered already. And copy the registration details, like the following,

* Organization-ID = [Your Organization ID]
* Device-Type = [Your Device Type]
* Device-ID = [Your Device ID]
* Authentication-Method = token
* Authentication-Token = [Your Device Token]

We need these details to connect the device to IBM Watson IoT Platform.

----


### Build & Run the sample using Eclipse

You must have installed the [Eclipse Maven plugin](http://www.eclipse.org/m2e/), to import & run the samples in eclipse. Go to the next step, if you want to run manually.

* Clone the iot-device-samples project using git clone as follows,

    `git clone https://github.com/ibm-messaging/iot-device-samples.git`
    
* Import the **device-management-sample** project into eclipse using the File->Import option in eclipse.

* Modify the **DMDeviceSample.properties** file with the device registration details that you noted in the above step.

* Build & Run each of the sample by right clicking on the project and selecting "Run as" option.

* Observe that the device connects to IBM Watson IoT Platform and lists down various device management operations that the sample agent can perform. Refer to [this recipe](https://developer.ibm.com/recipes/tutorials/connect-raspberry-pi-as-managed-device-to-ibm-iot-foundation/) for more information about how to run the RasPiDMAgent Sample.

----

### Building the sample - Required if you want to run the samples outside of Eclipse

* Clone the device-samples project using git clone as follows,
   
    `git clone https://github.com/ibm-messaging/iot-device-samples.git`
    
* Navigate to the device-samples project, 

    `cd iot-device-samples\java\device-management-sample`
    
* Run the maven build as follows,

    `mvn clean package`
    
This will download the Java Client library for Watson IoT Platform (Currently its shipped as part of this sample, but soon it will be made available in maven central repository), download all required dependencies and starts the building process. Once built, the sample can be located in the target directory, for example, target\ibmiot-device-management-sample-0.0.1.jar.

----

### Running the SampleRasPiDMAgent sample outside Eclipse

* Navigate to **target/classes** directory and modify the **DMDeviceSample.properties** file with the device registration details that you noted in the above step.

* Run the sample using the following command,

    `mvn exec:java -Dexec.mainClass="com.ibm.iotf.sample.devicemgmt.device.SampleRasPiDMAgent"`

**Note:** If there is an Error, try extracting the ibmwiotp.jar present in target/classes directory to the same location and run again. Remember the jar must be extracted in the same location. 

* Observe that the device connects to IBM Watson IoT Platform and lists down various device management operations that the sample agent can perform. Refer to [this recipe](https://developer.ibm.com/recipes/tutorials/connect-raspberry-pi-as-managed-device-to-ibm-iot-foundation/) for more information about how to run the RasPiDMAgent Sample.

----

**Note**: Follow the above steps to run any other samples present in this project.
