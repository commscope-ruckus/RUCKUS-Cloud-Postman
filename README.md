# Ruckus Cloud Postman collection
Use this collection to assist in the development of apps using Ruckus Cloud. You need to input your
tenantId, username, password and AP serial number at the tab "Variables". The other variables will be 
assigned automatically by the scripts in this collection.

Note: Ruckus Cloud write-APIs can be asynchronous. A response of 202 indicates an asynchronous 
response. That needs to be considered when writing API calls using python or any other language. 
Please refer to Ruckus Cloud python examples in this repository for details.

Any other response indicates a synchronous response. The read-APIs are always synchronous.
