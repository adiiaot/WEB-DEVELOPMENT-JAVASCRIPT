# JAVASCRIPT ARITHMETIC OPERATORS

*Arithmetic Operators* take numerical values as their operands and return a single numerical value.

In JavaScript, there are 8 basic arithmetic operators:

*OPERATORS* 
+ (Addition)
- (Subtraction)
* (Multiplication)
/ (Division)
** (Exponentiation)
% (Remaider)
++ (Increment)
-- (Decrement)

# ADDITION OPERATOR (+)
The addition operator (+) returns the sum of its numerical operands.

<script>
    var x = 3 + 3; //returns 6
    document.write(x); //prints out 6
</script>

*NOTE: The values 3 and 3 which were added together are called *operands*

HERE IS ANOTHER EXAMPLE:

<script>
    var x = 3 + 3 + 2; //returns 8
    document.write(x); //prints out 8
</script>

The addition operator can also be used to concatenate or add strings together.

<script>
    var text = "Making";
    var text1 = "Serious";
    var text2 = "Progress";

    var sentence = text + " " + text1 " " + text2;
    document.write(sentence); //prints out "Making Serious Progress"
</script>

HEAD OVER TO Addition-Operator (addition-operator.html) FOLDER TO SEE THE OUTPUT OF THIS CODE IN YOUR BROWSER 

(Turn on the LIVE SERVER or Run the code)
---------------------------------------------------------------------


# SUBTRACTION OPERATOR (-)
The Subtraction operator (-) returns the difference of its numerical operands.

<script>
    var x = 3 - 2; //returns 1
    document.write(x);
</script>

HEAD OVER TO Subtraction-Operator (subtraction-operator.html) Folder TO SEE THE OUTPUT IN YOUR BROWSER 
---------------------------------------------------------------------


# MULTIPLICATION OPERATOR (*)
The Multiplication operator (*) returns the product of its numerical operands.

<script>
    var x = 3 * 2; //returns 6
    document.write(x); //prints out 6 
</script>

HEAD OVER TO Multiplication-Operator (multiplication.html) FOLDER TO SEE THE OUTPUT IN YOUR BROWSER
---------------------------------------------------------------------

# DIVISION OPERATOR (/)
The division operator (/) returns the quotient of its numerical operands.

Where the left operand is the dividend and the right operand is the divisor.

<script>
    var x = 10 / 2; //returns 5
    document.write(x); //prints out 5
</script>

HEAD OVER TO Division-Operator (division.html) FOLDER TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------


# EXPONENTIATION (**)
The exponentiation operator (**) returns the result of raising its first operand to the power of its second operand 

HERE'S AN EXAMPLE

2 ** 4 (2 raised to the power of 4 which is 16)

<script>
    var x = 2 ** 4; //same as 2 * 2 * 2 * 2
    document.write(x); //prints 16
</script>

HEAD OVER TO Exponentiation-Operator (exponent.html) FOLDER TO SEE THE OUTPUT IN YOUR BROWSER
---------------------------------------------------------------------


# REMAINDER (%)
The Remainder operator (%) returns the remainder left when the first operand is divided by the second operand.

<script>
    var x = 5 % 2; // 5 divided by 2 is 2 remainder 1
    document.write(x); //prints the remainder 1
</script>

HEAD OVER TO Remainder-Operator (remainder.html) FOLDER TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------


# INCREMENT (++)
The Increment operator (++) adds 1 to its operand and returns a value.

<script>
    var x = 2;
    x++; //adds 1 to x
    document.write(x); //prints 3
</script>

HEAD OVER TO Increment-Operator (increment.html) FOLDER TO SEE THE OUTPUT OF THIS CODE IN YOUR BROWSER
---------------------------------------------------------------------


# DECREMENT (--)
The Decrement operator (--) deducts 1 from its operand and returns a value.

<script>
    var x = 2; 
    x--; //deducts 1 from x
    document.write(x); //prints 1
</script>

HEAD OVER TO Decrement-Operator (decrement.html) FOLDER TO SEE THE ... you know the drill.
---------------------------------------------------------------------

# OPERATOR SEQUENCE #

Operator sequence describes the order of performed operations in an arithmetic expression.

<script>
    var x = 10 + 2 * 3; //returns 16
    document.write(x); //prints out 16
</script>

HEAD OVER TO Operator-Sequence (operator.html) TO SEE THIS CODE OUTPUT

* As you may have notice the result of the expression above is 16.

WHY?

It is because *multiplication* is performed first before *addition*.

2 * 3 = 6, and then 10 + 6 = 16.

JavaScript follows the *MDAS* pattern in Math, where *multiplication* is performed first, *division* is second, *addition* is third and *subtraction* is fourth or last.

But what if we need a certain operation to be performed first?

* Let's say we want addition to be performed first in out previous example?

We can use the *grouping* to do that, grouped expressions are performed first before the others.

Use parenthesis () to group expressions.

<script>
    var x = (10 + 3) * 2; //returns 26
    document.write(x); 
</script>

HEAD OVER TO Operator-sequence (grouping.html) TO SEE THE OUTPUT