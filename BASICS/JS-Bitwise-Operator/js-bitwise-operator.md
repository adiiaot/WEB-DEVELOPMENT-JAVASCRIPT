# JAVASCRIPT BITWISE OPERATOR
*Bitwise Operator* treat their operands as a sequence of 32 bits (loops and ones), rather than as *numbers*.

For Example, the decimal number 5 has a binary representation of 101.

Bitwise operators return numerical values.

# BITWISE *AND (|)* OPERATOR
Performs the *AND* operation on each pair of bits.

It return 1 only if both *a* and *b* are 1.

<script>
    var num1 = 0 | 0; //returns 0
    var num2 = 0 | 1; //returns 0
    var num3 = 1 | 0; //returns 0
    var num4 = 1 | 1; //returns 1
</script>

---------------------------------------------------------------------


# BITWISE *OR (|)* OPERATOR
Performs the *OR* operation on each pair of bits.

It returns 1 if either *a* and *b* is 1.

<script>
    var num1 = 0 | 0; //returns 0 
    var num2 = 0 | 1; //returns 1
    var num3 = 1 | 0; //returns 1
    var num4 = 1 | 1; //returns 1
</script>

--------------------------------------------------------------------


# BITWISE *XOR (^)* OPERATOR
Performs the *XOR* operation on each pair of bits.

It returns 1 if *a* and *b* are different.

<script>
    var num1 = 0 ^ 0; //returns 0
    var num2 = 0 ^ 1; //returns 1
    var num3 = 1 ^ 0; //returns 1
    var num4 = 1 ^ 1; //returns 1
</script>

---------------------------------------------------------------------


# BITWISE *NOT (-)* OPERATOR
Performs the *NOT* operation on each bit

*NOT* *a* yeilds the inverted value.

<script>
    var num1 = -0; //returns -1
    var num2 = -1; //returns -2
</script>