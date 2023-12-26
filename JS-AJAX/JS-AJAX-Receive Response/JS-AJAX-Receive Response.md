# RECEIVING OR HANDLING RESPONSE FROM SERVER
Before you send a request to a server, you should first provide a function that will handle the response.

The *onreadystatechange* property sets up a function that will handle the response.

It is an event handler that gets called when the *readyState* changes or when a response is received.

<script>
    httpRequest.onreadystatechange = writeContent;

    //make a request here after defining a 
    // function for onreadystatechange

    function writeContent(){
        //codes
    }
</script>

In this example, when the page receives a response from the server the *writeContent* function will be called.

Notice that it has no (), it is because we are only giving a reference to the function, rather than actually calling it.

# THE *readyState* and *status* PROPERTIES
The *readyState* lets us check if the response of the server is already received.

It returns a *number* value representing the state of the request.

0 - UNSENT - Client has been created
1 - OPENED - open() has been called
2 - HEADERS_RECEIVED - send() has been called
3 - LOADING - Downloading.
4 - DONE - Operation is complete.

To know if there is already a response, check if the *readyState* property equals 4.

<script>
    function writeContent(){
        if(httpRequest.readyState === 4){
            // the response was received
        }else {
            // not ready yet
        }
    }
</script>

After that, check if the status of the request is *successful* OR *unsuccessful*

This can be done using the *status* property.

If the *status* property is equal to 200, then the request is successful.

<script>
    if (httpRequest.status === 200){
        // the request is successful
    }else {
        // there was a problem wiht the request
        // for example, the response may have a 404 (not found)
        // or 500 (Internal Server Error) response code
    }
</script>


So far, this is the content of the *writeContent()* function.

<script>
    function writeContent(){
        if(httpRequest.readyState === 4){
            // the response was received
               if (httpRequest.status === 200){
                        // the request is successful
                     }else {
                            // there was a problem wiht the request
                            // for example, the response may have a 404 (not found)
                            // or 500 (Internal Server Error) response code
                        }
        }else {
            // not ready yet
        }
    }
</script>


# THE *responseText* PROPERTY
This returns the server response as a string of text.

<script>
    const response = httpRequest.responseText;
</script>

Use this property after checking the state of the request and the status of the response.

<script>
    function writeContent(){
        if(httpRequest.readyState === 4){
            // the response was received
               if (httpRequest.status === 200){
                        // the request is successful
                        const response = httpRequest.responseText;
                     }else {
                            // there was a problem wiht the request
                            // for example, the response may have a 404 (not found)
                            // or 500 (Internal Server Error) response code
                        }
        }else {
            // not ready yet
        }
    }
</script>

