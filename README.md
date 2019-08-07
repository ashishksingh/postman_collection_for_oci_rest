# POSTMAN COLLECTION FOR INVOKING Oracle OCI REST APIs
Associated blog post : https://link.medium.com/sCcFWZU68W and http://www.ateam-oracle.com/invoking-oci-rest-apis-using-postman 

Youtube : https://www.youtube.com/watch?v=8x1-3-k0poM

Download the repository's Postman collections and environment.

Import the environment into Postman using the ‘Import’ button at the top, and activate it by selecting it from the top right drop-down. 

Open and Edit the newly imported environment, and set the OCI REST variables tenancyId, authUserId, keyFingerprint and private Key.

Now import the two collections into Postman.

From the OCI_REST_INITIALIZATION collection, invoke the Initializer GET for ‘jsrsasign-all-min.js’ , which imports and initializes a required library jsrsasign for encryption and digital signatures. This is a one-time setup task.

That’s it!! Now you can use the other oci_rest_collection to invoke any OCI REST APIs. The collection provides a sample GET and POST request, which can be extrapolated to invoke any OCI REST API.

Just make sure that the OCI REST calls are executed as part of the OCI_REST_COLLECTION, as that collection contains the necessary javascript code to generate OCI’s authentication header
