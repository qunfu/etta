## Promotions receiver

User makes the `HTTP` `POST` request to the server with the attached `CSV` file. Server receives the request, parrse the `CSV` file into `JSON` object,  
erase storage, writes `JSON` object into the storage.  

## Promotions exposer

User makes the `HTTP` `GET` request to the server with existing promotion `ID`, server receives the request, pick the `ID` from the request,  
find the relevand promotion by `ID` in the storage and return it with `HTTP` response.

User makes `HTTP` `GET` request to the server with non-existing promotion `ID`, server receives the request, return `HTTP` response with `404` status code.