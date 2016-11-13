##HTTP Verbs
Get  
Post  
Delete  
Patch  
Put

##Information about Resource Code 
1xx Informational - Request received, continuing process  

2xx Success - This class of status codes indicates the action requested by the client was received, understood, accepted, and processed successfully.  

3xx Redirection - This class of status code indicates the client must take additional action to complete the request. Many of these status codes are used in URL redirection  

4xx Client Error - The 4xx class of status code is intended for situations in which the client seems to have erred. 

5xx Server Error - The server failed to fulfill an apparently valid request.

##HTTP Resource Code That May Be Useful 
* 201 Created -
The request has been fulfilled, resulting in the creation of a new resource.
* 404 Not Found -
The requested resource could not be found but may be available in the future. Subsequent requests by the client are permissible.
* 408 Request Timeout - 
The server timed out waiting for the request. According to HTTP specifications: "The client did not produce a request within the time that the server was prepared to wait. The client MAY repeat the request without modifications at any later time.
* 503 Service Unavailable -
The server is currently unavailable (because it is overloaded or down for maintenance). Generally, this is a temporary state.

##Resource Code 418  
418 I'm a teapot (RFC 2324)
This code was defined in 1998 as one of the traditional IETF April Fools' jokes, in RFC 2324, Hyper Text Coffee Pot Control Protocol, and is not expected to be implemented by actual HTTP servers. The RFC specifies this code should be returned by tea pots requested to brew coffee.[50] This HTTP status is used as an easter egg in some websites, including Google.com.[51]  
####[Link to wiki page with information] (https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)
