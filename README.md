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


Building and Running the samples
================================
This repository contains the samples which can be executed either within Eclipse environment or outside. Check the following [link](java/api-samples-v2/README.md) which guides you in the same
