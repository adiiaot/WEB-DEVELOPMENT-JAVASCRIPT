# JAVASCRIPT ASSIGNMENT OPERATORS

An Assignment operator assigns value to its left operand based on the value of its right operand

In JavaScript, there are 7 basic assignment operators

* ASSIGNMENT     x = y      (means x = y)
* ADDITION assignment    x += y   (means x = x + y)
* SUBTRACTION assignment  x -= y   (means x = x - y)
* MULTIPLICATION assignment  x *= y  (means x = x * y)
* DIVISION assignment x /= y    (means x = x / y)
* REMAINDER assignment x %= y   (means x = x % y)
* EXPONENTIATION assignment x **= y  (means x = x ** y)

# ASSIGNMENT (=)
The assignment operator assigns a value to a variable.

<script>
    var x = 2; //assigns 4 to x
    document.write(x);
</script>
---------------------------------------------------------------------

# ADDITION ASSIGNMENT (+=)
The Addition assignment operator *adds* the value of the left and right operand then assigns the *sum* to the left operand

<script>
    var x = 2;
    var y = 2;
    x += y; //adds 2 and 2 together then assigns the sum to x
    document.write(x); //prints out 4
</script>

HEAD OVER TO Addition-assignment-Operator (addition-assignment.html) FOLDER TO SEE THE OUTPUT

* It can also be used to *concatenate* or add strings together.

<script>
    var x = "Making";
    var y = "Progress";
    x += y; //joins the variables to form "making progress"
    document.write(x); // prints "MakingProgress"
</script>

*DO THIS YOURSELF* Try writing this script in the addition-assignment.html File and run it to see the output
---------------------------------------------------------------------

# SUBTRACTION ASSIGNMENT (-=)
The Subtraction assignment operator *subtracts* the value of the right operand from the left operand and then assigns the *difference* to the left operand variable.

<script>
    var x = 4;
    var y = 2;
    x -= y; //deducts 2 from 4
    document.write(x); //prints 2
</script>

HEAD OVER TO Subtraction-assignment-Operator (subtraction-assignment.html) File TO SEE THE OUTPUT
---------------------------------------------------------------------


# MULTIPLICATION ASSIGNMENT (*=)
The Multiplication assignment operator *multiplies* the value of the left operand and right operand then assigns the *product* to the variable.

<script>
    var x = 2;
    var y = 2;
    x *= y; //2 multiplies 2
    document.write(x); //prints out 4
</script>

HEAD OVER TO Multiplication-assignment-Operator (multiplication-assignment.html) FILE TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# DIVISION ASSIGNMENT (/=)
The Division assignment operator *divides* the value of the left operand by the right operand and then assigns the *quotient* to the variable.

<script>
    var x = 10;
    var y = 2;
    x /= y; //10 divided by 2
    document.write(x); //prints the variable quotient 5
</script>

HEAD OVER TO Division-assignment-Operator (division-assignment.html) FILE TO SEE THE OUTPUT
---------------------------------------------------------------------


# REMAINDER ASSIGNMENT (%=)
The remainder assignment operator *divides* a variable by the value of the right operand and assigns the *remainder* to the variable.

<script>
    var x = 7;
    var y = 3;
    x %= y; //7 divided by 3 is 2 remainder 1
    document.write(x); //prints out 1
</script>

HEAD OVER TO Remainder-assignment-Operator (remainder-assignment.html) FILE TO SEE THE OUTPUT
---------------------------------------------------------------------

# EXPONENTIATION ASSIGNMENT (**=)
The exponentiation assignment operator *raises* the value of the left operand to the power of the right operand and assigns the value to a variable.

<script>
    var x = 2;
    var y = 4;
    x **= y; //2 raised to the power of 4 (2 * 2 * 2 * 2)
    document.write(x); //prints out 16
</script>

HEAD OVER TO Exponentiation-assignment-Operator (exponentiation-assignment.html) FILE TO SEE THE OUTPUT OF THIS CODE
------------------------------------------------------------------------------------------------------------------------------------------


# ADVANCED ASSIGNMENT OPERATORS
Here are the other assignment operators:

* Left shift assignment    x <<= y  (x = x << y)
* Right shift assignment   x >>= y  (x = x >> y)
* Unsigned right shift assignment   x >>>= y   (x = x >>> y)
* Bitwise AND assignment     x &= y    (x = x & y)
* Bitwise XOR assignment     x  ^= y    (x = x ^ y)
* Bitwsie OR assignment       x |= y     (x = x | y)