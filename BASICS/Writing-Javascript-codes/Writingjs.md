# WRITING JAVASCRIPT CODES

JavaScript codes should be written inside the <script> element.

<script>
    document.write("I am making progress");
</script>
---------------------------------------------------------------

But where should we put the <script> element?

*INTERNAL JAVASCRIPT*
The <script> element can either be placed in the <head> or in the <body> 
or you can place it in both.

BUT I RECOMMEND PLACING IT AFTER THE BODY TAG, it just looks organized that way and i've been using it that way for external js files.

HOWEVER THERE IS A DIFFERENCE

LOOK AT THE CODE SNIPPET BELOW!

*JAVASCRIPT IN <head>*

<!DOCTYPE html>
<html>
<head>
    <title> JAVASCRIPT IN THE HEAD TAG</title>
    <script type = "text/javascript">
/*add your js codes here*/    
    </script>
</head>
<body>
    <!---add your elements codes here--->
</body>
</html>
--------------------------------------------------------------------

*JAVASCRIPT IN <body>*

<!DOCTYPE html>
<html>
<head>
    <title> JAVASCRIPT IN THE HEAD TAG</title>
</head>
<body>
    <!---add your elements codes here--->
    <script type = "text/javascript">
/*add your js codes here*/    
    </script>
</body>
</html>

--------------------------------------------------------------

# WHAT'S THE DIFFERENCE?
When the <script> is inside the <head>, it loads first before the content of the page.

(THIS IS USEFUL FOR AUTHENTICATION/POPUPS )

When the <script> is inside the <body>, it loads after the content of the page (HTML elements) loads before the functions.

(THIS IS USEFUL FOR LETTING USERS SEE THE PAGE FIRST BEFORE THEY CAN CLICK ON ANYTHING)


* EXTERNAL JAVASCRIPT*

JavaScript can also be placed in external files.

JavaScript files have the file name extension of .js
e.g "script.js", "main.js", "any name you want.js"

HERE'S AN EXAMPLE BELOW!

<!DOCTYPE html>
<html>
<head>
<title>TRY IT OUT</title>
<script src="script.js"></script>
</head>
<body>
    <p id="demo">I UNDERSTAND JAVASCRIPT FILE EXTENSIONS</p>
    <button type="button" onclick="myFunc()">CHANGE VALUE</button>
</body>
</html>


*THE script.js FILE WILL CONTAIN CODES SUCH AS:

function myFunc(){
    document.getElementById("demo").innerHTML = "I CAN NAME JS FILE EXTENSIONS";
}

---------------------------------------------------------------------

As you have noticed, we placed the script.js file in the <head> tag, you can also place it in the <body> tag if you don't want the js file to load before the HTML elements.

THE EXTERNAL JS FILE can be placed inside a FOLDER named "js", if so you can add the file extension into the <html> file with the code snippet below!

<script src="js/script.js"><script>