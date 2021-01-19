# IRISDocDBRESTAPIPostmanCollectionSample
A Postman Collection of REST API calls to demonstrate InterSystems IRIS DocDB basic calls

See InterSystems Developer Community Post for more details:

For the benefit of those who want to use the Document Database (DocDB) capabilities within InterSystems IRIS, and specifically the REST API it provides, I put together a Postman Collection that provides samples for several basic calls.

The example uses "Color" documents, e.g. Red, Blue, etc, using a sample JSON structure from here.

The Collection includes calls of different "categories" -

* Create Metadata - create the database and related properties
* Get Metadata - understand what databases and properties are defined
* CUD - create/update/delete of Documents
* Find & Get Documents - retrieve documents according to ID or certain values or criteria
* Delete Metadata - delete properties or databases

The order in which the requests are in the Collection have some internal logic (e.g. first create the database and properties, then insert some data, then retrieve it), but of course you can use it in any order or changes you like.

The order also works well if running the Postman Collection Runner. I added some basic test scripts that allow Postman to display Passed or Failed status for each call.

Please note the last call *deletes all the document databases within a Namespace* - so **do not run this unless you really mean to**... not manually and not as part of running the whole Collection.

In order to make the calls work on various environments I used Postman's variables feature.

This allows you to change the server name/IP, the port, and the namespace.
