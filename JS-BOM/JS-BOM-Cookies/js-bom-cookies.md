# JAVASCRIPT BOM COOKIES
A web cookie or a cookie is a *small piece of data* that a server sends to a user's browser.

The browser may store it and send it back to the same server with the next request.

Cookies are used for these purposes:

* Session management - Logins, shopping carts, game scores or anything else the server should remember.

* Personalization - user preferences, themes and other settings
 
* Tracking - recording and analyzing user behaviour

# CREATING A COOKIE
To create a cookie, use the *document.cookie* property

It can be created like this:

<script>
    document.cookie = "name=value";
</script>

FOR EXAMPLE:

<script>
    document.cookie = "firstName=Ayo";
</script>

To create multiple cookies, separate the *name=value* pairs with a semicolon(;).

<script>
    document.cookie = "firstName=Ayo; lastName=Deji";
</script>

Cookies are deleted when the browser is closed.

Add an expiry date(in UTC) so that is does not get deleted when the browser is closed.

<script>
    document.cookie = "firstName=Ayo; lastName=Deji, expires=Mon, 21 Apr 2025 12:00:00 UTC";
</script>


# GETTING A COOKIE VALUE
The *document.cookie* property returns a string that contains all the cookies.

<script>
    //returns a string containing all cookies
    const cookies = document.cookie;
</script>

# CHANGING A COOKIE VALUE
To change a cookie's value, do the same way as you create it but with a different value.

<script>
    document.cookie = "firstName=AOT;
</script>

# DELETING A COOKIE
To delete a cookie, set the its *name* to an empty value and use *max-age=0.

<script>
    document.cookie = "firstName=; max-age=0";
</script>