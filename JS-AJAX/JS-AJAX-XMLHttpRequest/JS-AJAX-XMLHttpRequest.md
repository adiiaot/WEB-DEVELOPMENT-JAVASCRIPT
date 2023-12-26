# THE XMLHttpRequest OBJECT
AJAX uses the *XMLHttpRequest* object to send and receive data from a server.

The code below will create an XMLHttpRequest object:

<script>
    const variableName = new XMLHttpRequest();
</script>

FOR EXAMPLE:

<script>
    const httpRequest = new XMLHttpRequest();
</script>

Now, we use this object to make HTTP requests to a server.

# THE *XMLHttpRequest* PROPERTIES
This object contains the following properties:

* onreadystatechange - An event handler that is called whenever the *readyState* property changes.

* readyState - Returns the state of the request.

* responseType - Returns value that defines the response type.

* responseText - Returns the text received from a server following a request being sent.

* status - Returns the numerical HTTP status code of the XMLHttpRequest's response

* statusText - Returns a string containing the response string returned by the HTTP server.

# THE *XMLHttpRequest* METHODS
The XMLHttpRequest object contains the following methods:

* open() - initializes a request

* send() - sends a request

* abort() - Aborts a request if it has already been sent.

* getAllResponseHeader() - Returns all the response headers

* getResponseHeader() - Returns the string containing the text of the specified header

* setRequestHeader() - Sets the value of an HTTP request header.