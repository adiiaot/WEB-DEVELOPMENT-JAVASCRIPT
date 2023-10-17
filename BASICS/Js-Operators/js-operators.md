# JAVASCRIPT OPERATORS

JavaScript operators are used to perform particular actions.

They can be used to assign values, compare values, combine and perform arithmetic operations and more.

JavaScript operators symbols (or set of symbols) or keywords.

There are different types of operators.

*NOTE: There are different folders that explains all these operators in depth, but this is to help you familiarize with the concepts of each type.*

# ASSIGNMENT OPERATORS
The *assignment operator* is used to assign a value to a variabe.
It uses the equal = symbol.

<script>
    var x = 2; //assigns number 2 to x
    var y = 5; //assigns number 5 to y
    var sum = x + y; //assigns the sum of x and y to be added
    document.write(sum); //prints the sum
</script>

The *addition assignment* operator adds the value of the right operand to the value of the variable.

* Operator: x += y is 
* Equivalent to: x = x + y

HERE'S AN EXAMPLE
<script>
    var x = 2;
    var y = 5;

    x += y; //adds the value of y to x and then assigns the result to x

    document.write(x); //prints 7
</script>
---------------------------------------------------------------------

# ARITHMETIC OPERATORS
The *arithmetic operators* are used to perform arithmetic operations like (addition, subtraction, multiplication and division) between values.

HERE ARE THE SYMBOLS OF THE ARITHMETIC OPERATORS
* Addition: +
* Subtraction: - 
* Multiplication: *
* Division: /

*ADDITION* 
<script>
    var num1 = 3;
    var num2 = 2;
    var sum = num1 + num2; //adds the number 3 and 2
    document.write(sum); //prints out 5
</script>

*SUBTRACTION*
<script>
    var num1 = 3;
    var num2 = 2;
    var difference = num1 - num2; //deducts 3 from 2
    document.write(difference); //prints out 1
</script>

*MULTIPLICATION*
<script>
    var num1 = 3;
    var num2 = 2;
    var product = num1 * num2; //multiplies 3 times 2
    document.write(product); //prints out 6
</script>

*DIVISION*
<script>
    var num1 = 3;
    var num2 = 2;
    var quotient = num1 / num2; //divides num2 to num1
    document.write(quotient); //prints out 1
</script>

---------------------------------------------------------------------


# STRING OPERATORS
String operators are used to concatenate or add strings.

The *addition* operator + and the *addition assignment* operator += are the string operators.


* USING THE ADDITION OPERATOR
<script>
    var firstName = "Adii";
    var lastName = "Aot";

    var fullName = firstName + lastName;
    document.write(fullName); //prints out "Adii Aot"
</script>

* USING THE ADDITION ASSIGNMENT OPERATOR
<script>
    var firstName = "Adii";
    var lastName = "Aot";

    firstName += lastName;
    document.write(firstName); //prints out "Adii Aot"
</script>


We can also concatenate three or more strings.

<script>
    var text = "Making";
    var text1 = "serious";
    var text2 = "progress";

    var sentence = text + text1 + text2; //concatenates the three strings (joins all strings together to form a sentence)

    document.write(sentence); //prints out "Makingseriousprogress"
</script>

HEAD OVER TO concatenate.html TO SEE THE OUTPUT IN YOUR BROWSER

---------------------------------------------------------------------


# COMPARISON OPERATORS
Comparison operators compare its operand and returns a *Boolean* based on whether the comparison is *true* or *false*.

IN THE EXAMPLE BELOW, THE equality comparison operator is used to compare two numbers.

<script>
    var x = 2;
    var y = 2;

    document.write(x == y); //prints true because x is the same number as y
</script>

HEAD OVER TO comparison.html TO SEE THE OUTPUT IN YOUR BROWSER
---------------------------------------------------------------------


# LOGICAL OPERATORS
Logical operators are typically used with Boolean values.

They are used to determine the logic between its operands.

You will learn about logical operators in depth later in another folder in this course.

# BITWISE OPERATORS
A bitwise operator treats its operands as a set of 32 bits or zeros and ones.

It performs its operations on binary representations.

It returns numerical values.

You will learn about Bitwise operators in depth later in another folder in this course.