# RUCKUS Cloud JWT API New Endpoints
This collection uses the new endpoints.
Use this collection to assist in the development of apps using RUCKUS Cloud or R1.
You need to enter your credentials in the body of the /token call. This API uses JSON Web Token for authentication.
Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, network ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
call. That needs to be considered when writing API calls using python or any other language. 
Please see examples in the repository RUCKUS-Cloud-Python-Scripts for details.
Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud MSP JWT API New Endpoints
This collection uses the new endpoints.
This collection shows how to manage delegated accounts in RUCKUS Cloud or R1. It uses a MSP/MSP-EC delegation as an example.
You need to enter the MSP credentials in the body of the /token call. This API uses JSON Web Token for authentication, but in addition, when managing delegated accounts (i.e. the MSP-EC), you need to do two additional things: a) use the tenantId for the MSP-EC in the URL; b) add a request header with a key named x-rks-tenantid and the value as the MSP-EC tenantId. 

Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
call. That needs to be considered when writing API calls using python or any other language. 
Please see examples in the repository RUCKUS-Cloud-Python-Scripts for details.
Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud JWT API
This collection still uses many of the old endpoints (same as the collection which uses AP-KEY).
Use this collection to assist in the development of apps using RUCKUS Cloud.
You need to enter your credentials in the body of the /token call. This API uses JSON Web Token for authentication.
Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, network ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
call. That needs to be considered when writing API calls using python or any other language. 
Please see examples in the repository RUCKUS-Cloud-Python-Scripts for details.
Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud MSP JWT API
This collection still uses many of the old endpoints (same as the collection which uses AP-KEY).
This collection shows how to manage delegated accounts in RUCKUS Cloud. It uses a MSP/MSP-EC delegation as an example.
You need to enter the MSP credentials in the body of the /token call. This API uses JSON Web Token for authentication, but in addition, when managing delegated accounts (i.e. the MSP-EC), you need to do two additional things: a) use the tenantId for the MSP-EC in the URL; b) add a request header with a key named x-rks-tenantid and the value as the MSP-EC tenantId. 

Many variables will be assigned automatically by the scripts in this collection, using Pre-request Script and Tests in Postman. Change the variable values as appropriate (for instance, the AP and ICX switch serial number, ssid, etc)

Note: Many RUCKUS Cloud write-APIs are asynchronous. A response of 202 indicates an asynchronous 
call. That needs to be considered when writing API calls using python or any other language. 
Please see examples in the repository RUCKUS-Cloud-Python-Scripts for details.
Any other response indicates a synchronous response. The read-APIs are always synchronous.


# RUCKUS Cloud Postman collection (uses API-KEY - Deprecated)
Use this collection to assist in the development of apps using Ruckus Cloud. You need to input your
tenantId, username, password and AP serial number at the tab "Variables". The other variables will be 
assigned automatically by the scripts in this collection.

Note: Ruckus Cloud write-APIs can be asynchronous. A response of 202 indicates an asynchronous 
response. That needs to be considered when writing API calls using python or any other language. 
Please refer to Ruckus Cloud python examples in the repository Ruckus-Cloud-Python-Scripts for details.

Any other response indicates a synchronous response. The read-APIs are always synchronous.

# RUCKUS Cloud with MSP-EC calls (uses API-KEY - Deprecated)
This collection shows how to manage the customer objects in a MSP account.
MSP accounts have different security contexts for the MSP and the customers managed by the MSP. After retrieving the API token using the MSP credentials, you will only be able to do things at the MSP level.
There is an additional call to switch to a customer tenant, in order to be able to manage the customer objects:
 
{{baseUrl}}/api/login/tenant/token/{{customerId}}
 
After that, you can access or change the customer objects.


