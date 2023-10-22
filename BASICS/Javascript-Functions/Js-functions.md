# JAVASCRIPT FUNCTIONS
*Functions* are one of the fundamental building blocks of JavaScript.

A function is a *JavaScript method*.

It is a set of statements that performs a task or produces a value.

It is executed when it is *invoked* (called) by something.

# FUNCTION DEFINITION
A JavaScript function is defined or declared using the *function* keyword, followed by:

* The name of the function

* A list of parameters (optional) enclosed in parentheses (). Multiple parameters are seperated by commas (,).

* The block of codes or the statements enclosed in curly braces {}.

HERE IS THE SYNTAX:

<script>
    function functionName (parameter1, parameter2, parameter3){
        //codes or statements to be executed
    }
</script>

Parameters act as *placeholder variables* inside the function.

When the functionis called, the variables are assigned to the *arguements* (values) provided when the function is called.

<script>
    /* defining function */
    function writeText (str) {
        document.getElementById("demo").innerHTML = str;
    }

    writeText = "Making Progress!";
</script>

"Making Progress" gets printed out as *demo* is an Identifier to the <p> element in the HTML file
---------------------------------------------------------------------


# CALLING A FUNCTION
Functions will only be executed  when they are *called* or invoked

A function can be called inside a JavaScript program, just like what we did in the previous examples.

A function can be called when a event happens, most commonly when a button is clicked.
<!DOCTYPE html>
<html>
    <head>
        <title>CALLING A FUNCTION </title>
    </head>
    <body>
       <p id="demo">Sum will be printed here.</p>
       <button type=button onclick= "addNumbers(2, 5)"> ADD </button>
    </body>
</html>

<script>
    function addNumbers(num1, num2){
        var sum = num1 + num2;
        document.getElementById("demo").innerHTML = sum; //prints out 7
}
</script>

HEAD OVER TO Calling-A-Function (calling-function.html) TO SEE THE OUTPUT IN YOUR BROWSER

(*Before we move on, please be reminded that functions DON'T REQUIRE PARAMETERS.)

In the example below, the function's only task is to show a dialog box.

<script>
    function showDialog(){
        alert("Making Progress");
    }
</script>

* TIP: DO THIS YOURSELF (use a <button onclick="showDialog()">Click Me </button>)
in the HTML File to see the output in your browser
---------------------------------------------------------------------


# THE RETURN STATEMENT
The *return* statement is used in a function to STOP its execution and to RETURN a value to the *function caller*.

For example, the addNumbers() function below returns the *sum* of its arguements to the function caller.

Then, the function caller prints the returned value to an element.

<script>
    function addNumbers(num1, num2){
        var sum = num1 + num2;
        return sum;


        /* the function caller */
        document.getElementById("demo").innerHTML = 
        addNumbers(2, 5);
    }
</script>

HEAD OVER TO Return-Statement (return.html) TO SEE THE OUTPUT

Another example;

<script>
    function addNumbers(num1, num2){
        var sum = num1 + num2;
        return sum;
    }
         
         /* function caller */
    document.write(addNumbers(2, 5));
</script>

HEAD OVER TO Return-statement (return2.html) TO SEE THE OUTPUT
---------------------------------------------------------------------


The example below assigns the returned value to a variable. The variable is then used in a statement.

<script>
    function getFullName(firstName, lastName){
        return firstName + " " + lastName;
    }

    var fullName = getFullName("Adii", "Aot");
    document.write(fullName);
</script>

HEAD OVER TO Return-Statement (return3.html) TO SEE THE OUTPUT
---------------------------------------------------------------------

# FUNCTION SCOPE
Variables declared inside a function are called *local variables*

Local variables can only be used outside, the value's data type is *undefined*.

Notice that nothing will be printed on the paragraph element (<p>) with the *demo1* id, because the name variable cannot be used outside the function.

<script>
    function getAge(age){
        var fullName = "Ayo Deji";

        //the fullName variable can be used here
        document.getElementById("demo").innerHTML = 
        fullName + " is " + age + " years old "
    }

    //the fullName variable cannot be used here
    document.getElementById("demo1").innerHTML = fullName;
</script>

HEAD OVER TO Function-Scope (function-scope.html) TO SEE THE OUTPUT

AS you may have noticed, the first sentence was "Ayo Deji is Undefined years old" 

That is because *age* wasn't assigned any value

AND the second sentence was blank, because we assigned the *fullName* variable outside the *function* scope.


Let's say you want to see the *age* value in the sentence, we will assign the variable *age* to a value

<script>
    function getAge(age) {
        var fullName = "Ayo Deji";
        var age = 17;

        document.getElementById("demo").innerHTML = 
        fullName + " is " + age + " years old ".
    }

    //the fullName and age variables cannot be used here
    document.getElementById("demo1").innerHTML = 
    fullName + " is " + age + " years old ".;
</script>

HEAD OVER TO Function-scope (function-scope2.html) TO SEE THE OUTPUT
---------------------------------------------------------------------


# GLOBAL VARIABLES
Global variables can be used by any function.

Global variables are variables declared outside a function.

For example, the *animal* variable below is declared outside a function.

Therefore, it can be used by any function.

<script>
    var animal = "lion";

    function myFunc() {
        document.getElementById("demo").innerHTML = "My favorite animal is " + animal;
    }
</script>

HEAD OVER TO Global-variable (global.html) TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------


# WHY USE FUNCTIONS?

Functions in JavaScript are just like tools in real life. They make coding easier. *for real*

Instead of writing a block of codes over and over again (JAVA), we can just reuse the same code many times.

The function below converts kilometer to miles.

<script>
    function toMiles(kilometer){
        var miles = kilometer * 0.62137;
        return kilometer + " kilometer/s " + "equals " + miles + " miles.";
    }

    //we can use the function toMiles as many times we want in our code
    alert(toMiles(3));
    document.getElementById("demo").innerHTML = toMiles(10);
</script>

HEAD OVER TO Using-Function.html TO SEE THE OUTPUT OF THIS CODE.