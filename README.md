# iot-platform-v2api-samples
This repository contains samples that interacts with IBM Watson IoT Platform using the platform API Version 2. Currently, there are samples for Java; information and instructions regarding the use of these samples can be found in their respective directories.

Supported functionalities
=========================
The WIoTP API supports the following functionality for applications:

1. View organization details.

2. Bulk device operations (list all, add, remove).  

3. Device type operations (list all, create, delete, view details, update).  

4. Device operations (list devices, add, remove, view details, update, view location, view management information).  

5. Device diagnostic operations (clear log, retrieve logs, add log information, delete logs, get specific log, clear error codes, get device error codes, add an error code).  

6. Connection problem determination (list device connection log events).  

7. Device management request operations (list device management requests, initiate a request, clear request status, get details of a request, get list of request statuses for each affected device, get request status for a specific device).  

8. Usage management (retrieve number of active devices over a period of time, retrieve amount of storage used by historical event data, retrieve total amount of data used).

9. Publish events on behalf of devices  

10. Service status queries (retrieve service statuses for an organization).  


Refer to [the Swagger document](https://docs.internetofthings.ibmcloud.com/swagger/v0002.html#/) for more information about the list of API's.   


Setup your development environment
==================================
This section explains how to set up your development environment to use the Watson IoT Platform Client Library for Java.

Pre-requisites

* [Java 8](https://java.com/en/download/)

* [Maven 3](https://maven.apache.org/download.cgi)

* [Watson IoT Client Library for Java](https://github.com/ibm-watson-iot/iot-java)

* Optionally [Eclipse IDE](https://www.eclipse.org)

* [Git](https://git-scm.com/downloads)

Steps to run the example
------------------------
1. Git clone this Repository  
`git clone https://github.com/ibm-watson-iot/iot-platform-apiv2-samples`  

2. Open your Eclipse IDE  

3. Right click in `Enterprise Explorer` view in Eclipse and select New Maven Project and select the folder wherein you had git cloned the Repository   

4. Right click on the imported Maven Project `ibmiot-apiv2-samples` and build the project   

5. Modify the properties file and run any of the source files  
