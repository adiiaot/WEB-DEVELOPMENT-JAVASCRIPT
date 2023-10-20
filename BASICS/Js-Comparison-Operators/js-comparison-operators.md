# JAVASCRIPT COMPARISON OPERATORS
A *comparison operator* compares its operands and returns a *Boolean* based on whether the comparison is *true* or *false*.

It can be used to compare strings, numbers, Booleans (logical), or Object values.

In JavaScript, there are 8 Comparison Operators:

1. Equality Operator       ==
2. Inequality Operator      !=
3. Identity Operator        ===
4. Non-Identity Operator    !==
5. Greater than Operator    >
6. Greater than or equal Operator  >=
7. Less than Operator       <
8. Less than or equal Operator     <=
---------------------------------------------------------------------

# EQUALITY OPERATOR (==)
The equality operator (==) returns *true* if its operands are EQUAL, otherwise it returns *false*.

<script>
    2 == 2; //returns true
    2 == 4; //returns false
    "2" == 2; //returns true
    "Making Progress" == "Making Progress"; //returns true
    "Making Progress" == "Takes Time"; //returns false
</script>

HEAD OVER TO Equality-Operator (Equality-Operator.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------

# INEQUALITY OPERATOR (!=)
The Inequality operator (!=) returns *true* if its operands are NOT EQUAL, otherwise it returns *false*.

<script>
    2 != 2; //returns false
    2 != 4; //returns true
    "2" != 2; //returns false
    "Making Progress" != "Making Progress"; //returns false
    "Making Progress" != "Takes Time"; //returns true
</script>

HEAD OVER TO Inequality-Operator (inequality.html) TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------


# IDENTITY OPERATOR
The Identity Operator (===) also known as *strict equality*
operator, returns *true* if its operands are *equal* and of the same type.

2 === 2; //returns true

The example above returns *true* because the two operands are equal and of the same type

NOTE: Same type refers to the operands *data types* (strings, numbers ...)

HEAD OVER TO Identity-Operator(identity.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------

# NON-IDENTITY OPERATOR (!==)
The non-identity operator (!==) also known as *strict inequality* operator, returns *true* if its operands are NOT OF THE SAME TYPE and/or NOT EQUAL.

"4" !== 4; //returns true

The example above returns *true* because the two operands are EQUAL and are NOT OF THE SAME TYPE

The example below returns *false* because the two operands are EQUAL and are of the SAME TYPE.

4 !== 4; //returns false

HEAD OVER TO Non-identity-Operator(non-identity.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# GREATER THAN OPERATOR (>)
The greater than operator (>) returns *true* if the left operand is *greater than* the right operand.

4 > 2; //returns true
2 > 4; //returns false
2.25 > 2.24 //returns true
2.24 > 2.25 //returns false

HEAD OVER TO Greater-Than-Operator (Greater-than.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# GREATER THAN or EQUAL OPERATOR (>=)
The greater than or equal operator (>=) returns *true* if the left operand is greater than or equal to the right operand.

4 >= 2; //returns true
2 >= 4; //returns false
2.25 >= 2.24; //returns true
2.24 >= 2.25; //returns false
4 >= 4; //returns true
2.25 >= 2.25 //returns true

HEAD OVER TO GreaterThan-Equal-Operator (greaterthan-equal.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# LESS THAN OPERATOR (<)
The less than operator (<) returns *true* if the left operand is less than the right operand.

4 < 2; //returns false
2 < 4; //returns true
2.25 < 2.24 //returns false
2.24 < 2.25 //returns true

HEAD OVER TO Less-Than-Operator (less-than.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# LESS THAN or EQUAL OPERATOR (<=)
The less than or equal operator (<=) returns *true* if the left operand is less than or equal to the right operand.

2 <= 4; //returns true
4 <= 2; //returns false
2.24 <= 2.25; //returns true
2.25 <= 2.24; //returns false
4 <= 4; //returns true
2.25 <= 2.25; //returns true

HEAD OVER TO LessThan-Equal-Operator (lessthan-equal.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


We have only showed the returned *Booleans* of the comparison operators.

And we have not yet made any use of it.

# HOW CAN COMPARISON OPERATORS BE USED?
Comparison operators are mostly used in *conditional statements*.

The most basic conditional statement is the *if statement*.

<script>
    if (5 == 5) {
        document.write("Making Progress");
    }
</script>
HEAD OVER TO (if.html) TO SEE THE OUTPUT OF THIS CODE

As you may have noticed from the output in your browser printed out "Making Progress". 

It is because the condition (which is 5 == 5) is *true*.

If the condition is false, "Making Progress" will not be printed.

<script>
    if (5 == 4) {
        document.write("Making Progress");
    }
</script>

HEAD OVER TO if-2.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------

WE WILL COVER MORE ON *Conditional statements* later in another folder.