# JAVASCRIPT EXCEPTION HANDLING
While programming with JavaScript, you may encounter different types of errors.

# WHAT IS AN EXCEPTION?
In JavaScript, an exception is thrown (generated) whenever an error occurs.

An exception can be a *string*, *number*, *Boolean* or an *object*.

# CATCHING AN EXCEPTION
In real life, when someone throws a ball, we can *catch* it.

Also, when JavaScript throws an *exception*, we can *catch* it.

We can do so by using the *try...catch* statement.
---------------------------------------------------------------------


# THE *try...catch* STATEMENT

The *try...catch* statement takes a block of statement to test.

The *catch* statement specifies one or more responses when an exception is thrown.

Syntax:

<script>
    try{
        // block of statements to test
    }
    catch(errorVariable){
        // codes to run when an exception is thrown
    }
</script>

The *errorVariable* holds the value of the *exception*.

<script>
    try{
        myFunction();
    }
    catch(err){
        document.getElementById("demo").innerHTML = err;
    }
</script>

HEAD OVER TO Try-Catch.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *throw* STATEMENT
The *throw* statement allows us to throw our custom exceptions.

We may throw different types of expression.

This example below throws different types of exceptions.

<script>
    throw "Error occurred!"; //a string
    throw "21"; // a number
    throw false; //a boolean 
    throw {errorText: "Error Occurred!"}; //an object
</script>

Here's an example of using it with *try...catch*

<script>
    try{
        throw "An Error Occurred, Please fix it!";
    }
    catch (err){
        document.getElementById("demo").innerHTML = err;
    }
    finally {
        alert("Making Progress");
    }
</script>

HEAD OVER TO Throw.html TO SEE THE OUTPUT OF THIS CODE
===========
===========
# ILLUSTRATIVE EXAMPLE

In this example, if the user is below *18* an exception will be thrown.

<script>
    var submit = document.getElementById("submit");

    submit.onclick = function(){
        var age = parseInt(document.getElementById("age").value);

        try{
            if(age < 18){
                throw "user must be 18 or above to enter";
            } else {
                document.getElementById("demo").innerHTML = "User is 18 or above";
            }
        } catch (err){
            document.getElementById("demo").innerHTML = err;
        }
    }
</script>

HEAD OVER TO Example.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# ERROR OBJECTS

*Error* objects are thrown when runtime errors occur.

The following are the different types of *Error*.

* ERROR NAME/Description - 

* *RangeError* (Error that occurs when a numeric variable or parameter is outside of its valid range.)

* *ReferenceError* (Error that occurs when de-referencing an invalid reference)

* *SyntaxError* (Error that occurs when parsing code in *eval()* method)

* *TypeError* (Error that occurs when a variable or paramater is not a valid type)

* *URIError* (Error that occurs when *encodeURI()* or *decodeURI()* are passed invalid parameters)

All the mentioned objects above contain the following properties:

*name* (returns the error name)
*message* (Returns the error message)
---------------------------------------------------------------------


# RangeError
The *RangeError* is thrown when a numeric variable or parameter is outside of its valid range.

For example, the *toExponential()* method only takes a *number* argument in the range between 0 and 100, if we give it a value outside that range, it will throw an exception.

<script>
    var number = 21.444;
    try{
        number.toExponential(-2);
    }
    catch (err){
        document.getElementById("name").innerHTML = err.name;
        document.getElementById("message").innerHTML = err.message;
    }
</script>

HEAD OVER TO RangeError.html
---------------------------------------------------------------------


# ReferenceError
The *ReferenceError* is thrown when de-referencing an invalid reference.

For example, since the *num2* variable does not exist, an exception is thrown.

<script>
    var num1 = 21.444;
    try {
        var total = num1 + num2;
    }
    catch (err){
        document.getElementById("name").innerHTML = err.name;
        document.getElementById("message").innerHTML = err.message;
    }
</script>

HEAD OVER TO ReferenceError.html 
---------------------------------------------------------------------


# SyntaxError
The *SyntaxError* is thrown while parsing code in *eval()* method.

For example, since the *string* below is not enclosed by quotes, an exception is thrown.

<script>
    try {
        eval("document.write('Making Progress)"); // must "Making Progress" to avoid error
    }
    catch (error){
        document.getElementById("name").innerHTML = error.name;
        document.getElementById("message").innerHTML = error.message;
    }
</script>

HEAD OVER TO SyntaxError.html
---------------------------------------------------------------------


# TypeError
The *TypeError* is thrown when a variable or parameter is not a valid type. 

For example, the *toFixed()* method can only be used on a *number* but we will use it on a *string*.

Because of that, an exception will be thrown.

<script>
    var text = "Making Progress";
    try {
        var x = text.toFixed(2);
    }
    catch (err){
        document.getElementById("name").innerHTML = err.name;
        document.getElementById("message").innerHTML = err.message;
    }
</script>

Head over to TypeError.html
---------------------------------------------------------------------


# URIError
The *URIError* is thrown when encodeURI() or decodeURI() are passed invalid parameters.

For example, when we provide an invalid character sequence (malformed URI) to the decodeURI() method, an exception will be thrown.

<script>
    try {
        var x = decode("%E0%A4%A");
    }
    catch (err){
        document.getElementById("name").innerHTML = err.name;
        document.getElementById("message").innerHTML = err.message;
    }
</script>

Head over to URIError.html