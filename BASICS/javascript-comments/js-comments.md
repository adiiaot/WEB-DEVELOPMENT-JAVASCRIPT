# JAVASCRIPT COMMENTS

JavaScript comments are used to make programming easier to read and understand.

Comments are not executed by the browser.

Comments can be used to add notes, suggestions and hints to a JavaScript code.

There are two types of comments in Javascript, the single-line and the Multi-line.

# SINGLE-LINE COMMENTS
To make a single-line comment, add two "//" to the beginning of the line.
This turns the texts turn into a comment, below is an example

<script>
    //this function changes the content of the p tag
    function myfunc(){
        var text = "Making Progress!";
        document.getElementById("demo").innerHTML = text; //replaces p id="demo" with text variable.
    }
</script>

Another way you can add a comment is by using the /* */, the comment goes between the asterisks.

This technique is much more flexible. Below is an example

<script>
    /* this is a comment on the code below */
    function myfunc(){
        var text = "Making Progress";
        document.getElementById("demo").innerHTML = text; /* replaces demo with text variable */
    }
</script>

// for speed and short comments
/* */ for flexiblity and design, you can also use this in the middle of a line

<script>
    function myfunc(){
        var x = 3;
        var y = 6;

        var sum = x + /* we will add y */ y; //adds 3 + 6
        document.getElementById("demo").innerHTML = sum; //prints out 9
    }
</script>

NOW DID YOU SEE WHAT I DID THERE, I used both single-line comments in the code and you can see how useful they are in programming.



# MULTI-LINE COMMENTS
To make multi-line comments, use this syntax

/* 
    This is a multi-line commenet
    This is a real multi-line
    I am useful for long comments
*/

LOOK AT THE CODE SNIPPET BELOW, and see how they are being used

<script>
    function myfunc(){
        var x = 4;
        var y = 4;
        var sum = x + y;

        /* let's add the value of x and y
        and then print out their sum */

        /* 
        you can comment like this sometimes
        it's more convenient and
        easier to read
        */
       document.getElementById("demo").innerHTML = sum;
    }
</script>

# DISABLING CODE USING COMMENTS
We can disable code using comments to prevent it from running.

This technique is helpful for testing purposes.

Let's say you just finished writing a piece of code and then you run it, later on you add another piece of code and the program stops functioning.

You can go back to the new code you added and turn it into a comment by adding the // or /* */ at the beginnig of the code line

BELOW IS AN EXAMPLE

<script>
    function myfunc(){
        var x = 4;
        var y = 5;
        var sum = x + y; //adds x + y
        var product = x * y; //multiplies y to x

        //document.getElementById("demo").innerHTML = sum;
        document.getElementById("demo").innerHTML = product;

        /* WE JUST DISABLED THE sum variable from executing 4 + 5
        now our output will be 4 * 5 which is 20
    }
</script>