# JAVASCRIPT STATEMENTS
JavaScript programs consist of statements with appropriate syntax.

A single JavaScript statement may span a single or multiple lines.

JavaScript statements should be ended or be separated by semicolons (;);

BELOW IS AN EXAMPLE OF A SINGLE LINE STATEMENT

* This statement writes the text "Making Progress" to the paragraph element(<p>) with the element (id) elem.

<!DOCTYPE html>
<html>
<head>
    <title>TRY IT OUT</title>
</head>
<body>
    <p id="elem">FIRST PARAGRAPH </p>
    <button type="button" onclick="myfunc()">CHANGE TEXTS</button>
</body>
    <script>
        document.getElementById("elem").innerHTML = "SECOND PARAGRAPH"; //THE FIRST PARAGRAPH changes into SECOND PARAGRAPH
    </script>
</html>

---------------------------------------------------------------------

*GROUPING JAVASCRIPT STATEMENTS*
JavaScript statements can be grouped inside curly brackets {...}

These are called "CODE BLOCKS"
Code blocks are used to make statements execute together.

They are commonly used in functions

<script>
    function myfunc() {
        document.getElementById("elem").innerHTML = "THIRD PARAGRAPH";
    }
</script>

---------------------------------------------------------------------

*JAVASCRIPT KEYWORDS*
Javascript statements usually start with a keyword.

Each keyword in Javascript has its own special meaning.

For example, in order to declare a variable, we have to use the "var" keyword.

<script>
    function myfunc(){
        var text = "FOURTH PARAGRAPH!";
        document.getElementById("elem").innerHTML = text;//replaces the THIRD PARAGRAPH TO FOURTH PARAGRAPH
    }
</script>