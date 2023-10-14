# JAVASCRIPT SYNTAX (JS SYNTAX)

JavaScript follows a set of rules called *syntax*

JavaScript syntax should be followed to create correctly-constructed programs.

# VARIABLE DECLARATION
In maths, we use variables to hold values.

It works the same way in JavaScript, a value can be assigned to a variable.

This is called declaring variables.

To declare a variable, use the "var" keyword to create it, and then an equal sign = to assign a value.

LOOK AT THE CODE SNIPPET BELOW

<script>
    var num = 4; //assigns the number 4 to the variable
    document.write(num); //prints out 4 as "num" is an identifier of the variable
</script>

The "num" in the code snippet example is called "identifier".

JavaScript identifiers are used to name variables.

# JAVASCRIPT IS CASE-SENSITIVE!
JavaScript identifiers are sensitively-cased.

Look at the code snippet below, in this example the variables "num" and "Num" are different!

<script>
    var num = 4;
    var Num = 8;

    var sum = num + Num; //adds 4 + 8, I bet you already understand
    document.write(sum); //prints out the value of sum which is 12
</script>

HEAD OVER TO syntax.html FILE to see the output of this code