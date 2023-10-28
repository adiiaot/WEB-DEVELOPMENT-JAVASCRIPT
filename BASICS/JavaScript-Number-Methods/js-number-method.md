# JAVASCRIPT NUMBER METHODS
The *Number* object provides methods that allow us to work with numerical values.

# THE *Number.isInteger()* METHOD
The *Number.isInteger()* method returns *true* if the passed arguement (value) is an integer.

<script>
    var num1 = Number.isInteger(21); //returns true
    var num2 = Number.isInteger(3.21); //returns false
    var num3 = Number.isInteger("Making"); //returns false
</script>

HEAD OVER TO Number-isInteger-Method (number-isInteger.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *isNaN()* METHOD
The *isNaN()* method returns *true* if the passed arguement (value) is *not a legal number*.

<script>
    var num1 = isNaN(21); //returns false
    var num2 = isNaN(3.21); //returns false
    var num3 = isNaN("Making Progress"); //returns true
    var num4 = isNaN("five"); //returns true
    var num5 = isNaN(12 / "five"); //returns true
</script>

HEAD OVER TO IsNaN-Method (isNaN.html) TO SEE THE OUTPUT
---------------------------------------------------------------------


# THE *parseInt()* METHOD
The *parseInt()* method takes a string arguement (value) and returns an integer based on the given value.

<script>
    var num1 = parseInt("21"); //returns 21
    var num2 = parseInt("2.22"); //returns 2
    var num3 = parseInt("22.2 days"); //returns 22
    var num4 = parseInt("22.2 months and 22 days"); //returns 22
    var num5 = parseInt("months 3"); //returns NaN
    var num6 = parseInt("Making Progress"); //returns NaN
</script>

HEAD OVER TO ParseInt-Method (parseInt.html) TO SEE THE OUTPUT

Notice that only the first number is returned if the next character are not numbers.

Also, it returns *NaN* if the arguement cannot be converted.
--------------------------------------------------------------------


# THE *parseFloat()* METHOD
The *parseFloat()* method takes a string arguement and returns a floating point number

<script>
    var num1 = parseFloat("21"); //returns 21
    var num2 = parseFloat("2.22"); //returns 2.22
    var num3 = parseFloat("22.2 days"); //returns 22.2
    var num4 = parseFloat("22.2 months and 22 days"); //returns 2
    var num5 = parseFloat("months 3"); //returns NaN
    var num6 = parseFloat("Making Progress"); //returns NaN
</script>

HEAD OVER TO ParseFloat-Method (parseFloat.html) TO SEE THE OUTPUT
---------------------------------------------------------------------


# THE *toFixed()* METHOD
The *tofixed()* method formats a number using fixed-point notation.

It returns a string with the specified number of decimals.

<script>
    var num1 = (21.123456).toFixed(1); //returns 21
    var num2 = (21.123456).toFixed(2); //returns 21.12
    var num3 = (21.123456).toFixed(3); //returns 21.123
</script>

HEAD OVER TO toFixed-Method (tofixed.html) TO SEE THE OUTPUT
---------------------------------------------------------------------


# THE *toExponential()* METHOD
The *toExponential()* method returns a string in exponential notation based on the given floating point.

<script>    
    var num1 = (55.1234).toExponential(1); //returns 5.5e+1
    var num2 = (55.1234).toExponential(2); //returns 5.51e+1
    var num3 = (55.1234).toExponential(3); //returns 5.512e+1
</script>

HEAD OVER TO toExponential-Method (toExponent.html) TO SEE THE OUTPUT
---------------------------------------------------------------------


# THE *toString()* METHOD
The *toString()* method returns a string representing the specified number.

<script>
    var num1 = (21).toString(); //returns "21"
    var num2 = (2.22).toString(); //returns "2.22"
    var num3 = (2023).toString(); //returns "2019"
</script>

HEAD OVER TO toString-Method (toString.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------
==============================================================================================================================================================================================================


# *NUMBER* PROPERTIES

* PROPERTY ----- * Description ----------* CONSTANT VALUE

1. NUMBER.MIN_VALUE > The smallest positive representable number in JavaScript.  5e-324

2. NUMBER.MAX_VALUE > The largest positive representable number in JavaScript. 1.7976931348623157e+308

3. NUMBER.NaN > Special "Not-A-Number" value. NaN

4. NUMBER.MIN_SAFE_INTEGER > The minimum safe integer in javaScript. -9007199254740991

5. NUMBER.MAX_SAFE_INTEGER > The maximum safe integer in JavaScript
9007199254740991