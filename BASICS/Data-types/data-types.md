# JAVASCRIPT DATA TYPES

In JavaScript or in any programming language, the concept of data types is important.

# WHAT ARE DATA TYPES?
Data types are the different kinds of data that can be stored or used in a JavaScript program.

# STRING DATA TYPE
The *string* data type is a sequence of characters used to represent text.

String can be written with either single or double quotes.

<script>
    var name = "Adii Aot"; //double quotes
    var name1 = 'Ayo Deji'; //single quotes

    document.getElementById("demo").innerHTML = name + "<br>", + name1;
</script>

---------------------------------------------------------------------

* SHOULD YOU USE SINGLE OR DOUBLE QUOTES?
You can use which one you like. I prefer double quotes sha.

But if the string contains single quotes, use double quotes
or if it contains double quotes, use single quotes

BELOW IS AN EXPLANATION 

<script>
    var sentence = "His name is 'Ayo Deji' "; //use double quotes
    var sentence1 = 'His name is "adii aot" '; //use single quotes

    document.getElementById("demo").innerHTML = sentence + "<br>" + sentence1;
</script>

HEAD OVER TO quotes.html FILE to see the output of this code
---------------------------------------------------------------------


# NUMBER DATA TYPE
The *number* data type is an *integer* or a *floating point* number (number with decimal).

<script>
    var x = 4; //an integer
    var y = 2.2; // a floating point number

    document.getElementById("demo").innerHTML = x + "<br>" + y; //outputs the value
</script>

HEAD OVER TO numberData.html FILE to see the output of this code

* ADDING TWO NUMBERS

We can also add the two numbers together,
<script>
        var x = 4; //an integer
        var y = 2.2; //a floating point number
        var sum = x + y; //adds x and y

        document.getElementById("demo").innerHTML = sum; //outputs 6.2
    </script>

HEAD OVER TO numberData2.html FILE to see the output.
---------------------------------------------------------------------

# COMBINING STRINGS AND NUMBERS
Combining a string and a string returns a *string*

Combining a number and a number returns a *number*

Combining a string and a number returns a *string* (just imagine!)

LOOK AT THE CODE SNIPPET BELOW

<script>
    var text = 17 + "Adiiaot"; //returns "17Adiiaot"
    var text1 = "Ayodeji" + 17; //returns "Ayodeji17"

    document.getElementById("demo").innerHTML = text + "<br>" + text1; //outputs 17Adiiaot Ayodeji17
</script>

HEAD OVER TO combineData.html to see the output in your browser

*NOTE: Since JavaScript evaluates from left to right, different sequences produce different results.

<script>
    var text = 21 + 2 + "Adiiaot"; //returns 23Adiiaot
    var text1 = "Ayodeji" + 21 + 2; //returns Ayodeji23

    document.getElementById("demo").innerHTML = text + "<br>" + text1; //outputs 23Adiiaot Ayodeji23
</script>

YOU CAN REPLACE THE SCRIPT FILE IN combine.html with this <script> code above to see the output.

---------------------------------------------------------------------

# BOOLEAN DATA TYPE
The *Boolean* data type is a logical data type that can only have *true* or *false* as values.


<script>
        var iscodingFun = "true";
        var iscopyPasteFun = "false";
    
        document.getElementById("demo").innerHTML = "is Coding Fun?" + " " + iscodingFun + "<br>" + "is Copy Paste Fun?" + " " + iscopyPasteFun;
</script>

HEAD OVER TO boolean.html FILE to see the output in your browser

Booleans are mainly used for conditional testing, not the one we did in the other example.

You will learn more about conditional testing in another folder.
Now back to booleans../

*Booleans* are the output of *comparison operators*

The == comparison operator tests if two values are equal or the same.
If they are equal, it returns *true*, otherwise *false*.

LOOK AT THE CODE BELOW TO UNDERSTAND MORE

<script>
    var x = 3;
    var y = 3;
    var areEqual = (x == y);//compares 3 and 3 to see if they are equal 

    document.getElementById("demo").innerHTML = areEqual;//returns true because 3 is equal to 3
</script>

HEAD OVER TO comparison.html FILE TO SEE THE OUTPUT
---------------------------------------------------------------------

# THE UNDEFINED DATA TYPE
If a variable has no assigned value, the value is *undefined*.

In the example below, the *title* variable is declared but is not assigned to any value.
Therefore, the value is undefined.

<script>
    var title;

    document.getElementById("demo").innerHTML = title; //outputs undefined
</script>

HEAD OVER TO undefined.html FILE TO SEE THE OUTPUT

---------------------------------------------------------------------

# THE NULL DATA TYPE

The *null* data type is a special data type denoting a null value, meaning it's not an empty string "" or 0.

It simply means nothing.

<script>
    var fruit = null;

    document.write(fruit); //prints null
</script>

We can empty a variable by setting it to null.

<script>
    var fruit = "apple";
    document.write(fruit + "<br>");//prints apple, but wait, let us remove it

    fruit = null; //sets the value to null
    document.write(fruit); //prints null
</script>

HEAD OVER TO null.html FILE TO SEE THE OUTPUT

---------------------------------------------------------------------


# OBJECT DATA TYPE
In this section we will only cover the basic concepts of Javascript *Objects*.

The Object data type is a collection of related data.

Object contain properties written in key: value pairs.

Each pair is separated by a comma (,).
Objects are written inside curly brackets {}.

<script>
    var banana = {
        color: "yellow",
        size: "long",
        quantity: 3,
        isSweet: true,
    };
</script>
HEAD OVER TO object.html TO SEE THE OUTPUT

In the example above, the *banana object* has 4 properties: *color*, *size*, *quantity* and *isSweet*.
---------------------------------------------------------------------


# JAVASCRIPT ARRAYS
A JavaScript array is a collection of values. Each value is separated with a comma (,).

It is written in square brackets [].

The data type of an array is *object*.
