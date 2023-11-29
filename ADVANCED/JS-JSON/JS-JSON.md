# JAVASCRIPT OBJECT NOTATION
JSON or JavaScript Object Notation is a standard text-based format for representing structured data based on JavaScript object syntax.

JSON is commonly used for sending data from the server to a client e.g a web page.

A JSON object can be stored in its own file, which is basically just a text file with an extension of *.json* e.g *fileName.json*.

*NOTE! JSON is basically just a text*

# JSON SYNTAX
JSON's syntax is closely similar to JavaScript objects.

When writing a JSON object, always take note of the following:

* JSON can NOT contain methods.

* JSON requires the use of double quotes ("), single quotes (') are not valid.

* A single misplaced comma will cause the JSON to not work.

* Property names in JSON should be enclosed by quotes.

Here's a basic example:

<script>
    {
        "firstName": "Ayo",
        "lastName": "Aot",
        "age": 17,
        "isMarried": true
    }
</script>

Notice that the example above contains a *string*, a *number* and a *Boolean*.

In the example below, the JSON contains an *object* and an *array*.

<script>
    {
        "favorites": {
            "food": "Rice",
            "game": "basketball",
            "color": "orange"
        },
        "hobbies": ["coding", "gaming", "chess"]
    }
</script>
=====================================================================


# CONVERTING JSON TO JAVASCRIPT OBJECT
To convert JSON  to a regular JavaScript object, use the *JSON.parse* method

*Commonly, a JSON is read from a server and stored in a variable*.

<script>
    const text = `{
        "firstName": "Ayo",
        "lastName": "Aot",
        "age": 18,
        "isMarried": true 
    }`;

    const obj = JSON.parse(text); // returns an object

    // now we can access its properties
    document.getElementById("demo").innerHTML = 
    obj.firstName + " " + obj.lastName + " is " + obj.age + " years old."; 
</script>

HEAD OVER TO JSON-js.html
---------------------------------------------------------------------


# CONVERTING JAVASCRIPT OBJECT TO JSON
To convert a regular JavaScript object to JSON, use the *JSON.stringify()* method.

<script>
    const text = `{
        "firstName": "Ayo",
        "lastName": "Aot",
        "age": 18,
        "isMarried": true 
    }`;

    const obj = JSON.stringify(text); // returns an JSON

    // now we can print the JSON text
    document.getElementById("demo").innerHTML = text; 
</script>

HEAD OVER TO JS-JSON.html

Commonly, a JSON text is sent to a server. And the server processes the JSON.