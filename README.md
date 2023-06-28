# RUCKUS Cloud & R1 JWT API New Endpoints
This collection uses the new endpoints.
Use this collection to assist in the development of apps using RUCKUS Cloud or R1.
You need to enter your credentials in the body of the /token call. This API uses JSON Web Token for authentication.
Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, network ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
call. That needs to be considered when writing API calls using python or any other language. 
Please see examples in the repository RUCKUS-Cloud-Python-Scripts for details.
Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud & R1 MSP JWT API New Endpoints
This collection uses the new endpoints.
This collection shows how to manage delegated accounts in RUCKUS Cloud or R1. It uses a MSP/MSP-EC delegation as an example.
You need to enter the MSP credentials in the body of the /token call. This API uses JSON Web Token for authentication, but in addition, when managing delegated accounts (i.e. the MSP-EC), you need to do two additional things: a) use the tenantId for the MSP-EC in the URL; b) add a request header with a key named x-rks-tenantid and the value as the MSP-EC tenantId. 

Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
call. That needs to be considered when writing API calls using python or any other language. 
Please see examples in the repository RUCKUS-Cloud-Python-Scripts for details.
Any other response indicates a synchronous response. The read-APIs are always synchronous.

# General Notes
- You need to enter your credentials in the /token call, and edit the serial number for the access point at /venues/aps and for the ICX switch at /switches.
- Older collections can be found in the archive folder.




