# SENDING REQUEST TO A SERVER
To send a request, you need to initialize a request first before sending it to a server.

The *open()* method initializes a request.

Syntax:

<script>
    XMLHttpRequest.open(method, url)
</script>

The *method* is the HTTP request method to use.

It can be *"GET"* or a *"POST"* method.

The *url* is a string representing the URL to send the request ot.

# SENDING A GET REQUEST
Use the "GET' method when sending *insensitive data*.

This will send a "GET" request to *https://example.com/best-server.php*.

<script>
    httpRequest.open("GET", "https://example.com/best-server.php");
    httpRequest.send();
</script>

The *send()* method will send the request to the server.

We can also send additional information with the *GET* request using URL parameters.

URL parameters look like this:

*?name1=value1&name2=value2.* 

FOR EXAMPLE:

<script>
    httpRequest.open("GET", "https://example.com/test-server.php?firstName=Ayo&lastName=Aot");
    httpRequest.send();
</script>


# SENDING A *POST* REQUEST
Use the *"POST"* method when sending *sensitive data* like passwords or any private personal information.

Sending a *"POST"* request is somehow similar to sending a "GET" request.

But you need to specify a request header using the *setRequestHeader()* method.

And you need to put the URL parameters inside the *send()* method, not with the *url* when you initialize a request.

<script>
    httpRequest.open("POST", "https://example.com/best-server.php");
    httpRequest.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");
    httpRequest.send("firstName=Ayo&lastName=Aot");
</script>