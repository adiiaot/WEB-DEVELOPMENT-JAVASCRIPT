# JAVASCRIPT BOM LOCATION
The *window.location* object is used to return information about the current location of the page.

Just like other *window* properties, it can be accessed without the *window* prefix.

The *location* object contains the following properties:

* href
* protocol
* hostname
* pathname

# THE *href* PROPERTY
The *href* property returns whole URL of the current page.

Let's say for example that this page is located at

https://www.example.com/pages/index.html

<script>
    const x = location.href;
    // x returns "https://www.example.com/pages/index.html"
</script>



# THE *protocol* PROPERTY
The *protocol* property returns the Protocol scheme of the URL of the page e.g "http:" and "https:"

<script>
    const x = location.protocol;
    // x returns "https:"
</script>



# THE *hostname* PROPERTY
The *hostname* property returns the domain name of the URL of the page.

<script>
    const x = location.hostname;
    //x returns "www.example.com"
</script>



# THE *pathname* PROPERTY
This returns the path of the URL of the page.

<script>
    const x = location.pathname;
    //x returns "/pages/index.html"
</script>