# JAVASCRIPT NUMBERS

In JavaScript, there are two types of numbers.

* Integer - number without decimals
* Floating Point - number with decimals

<script>
    var num1 = 2; //an integer
    var num2 = 2.15; //an floating point
</script>
---------------------------------------------------------------------

# EXTRA LARGE OR SMALL NUMBERS
Very large or small numbers can be written using *e-notation* (exponent notation).

<script>
    var num1 = 212e6; //or 21200000
    var num2 = 212e-6; //or .000212
</script>

---------------------------------------------------------------------


# STRING AS NUMBERS
JavaScript will try to convert *numbers* as much as possible.

<script>
    var difference = "10" - "2"; //returns 8
    var product = "10" * "2"; //returns 20
    var quotient = "10" / "2"; //returns 5
</script>


However, adding numbers as strings DOES NOT WORK IN ADDITION.
Instead, the addition operator will concatenate them as strings.

<script>
    var sum =  "10" + "2"; //returns 102 instead of 12
</script>
---------------------------------------------------------------------


# PERFORMING OPERATIONS ON STRINGS AND NUMBERS
Again, JavaScript will try to convert numbers as much as it possibly can.

This time, let's show examples where one number is a *number* and the other is a *string*

<script>
    var difference "10" - 2; //returns 8
    var product = 10 * "2"; //returns 20
    var quotient "10" / 2; //returns 5
</script>

As you may notice, the above examples worked.

It's because JavaScript was able to convert the *strings* to *numbers*

However, again, this does not work with *addition*. Because JavaScript CONCATENATES them as *strings* and DON'T ADD THEM AS NUMBERS.

<script>
    var sum = "10" + 2; //returns 102 again instead of 12
    var sum1 = 10 + "2"; //returns 102 AGAIN! instead of 12, see I told you
</script>

TRY TO RUN THIS CODE IN A NEW FILE AND CHECK IT IN YOUR BROWSER
---------------------------------------------------------------------

# HEXADECIMAL NUMBERS
Hexadecimal number syntax uses a leading 0 followed by a letter x.

Then followed by characters inside the range of 
(0123456789ABCDEF).

<script>
    var num1 = 0xA; //returns 10
    var num2 = 0xff; //returns 25
    var num3 = 0x123456789ABCDEF; //returns 81985529216486900
</script>
---------------------------------------------------------------------


# *NaN* - NOT A NUMBER
NaN means *Not-A-Number*. It is a property representing an illegal number.

Performing arithmetic operations with non-numeric data will return NaN.

<script>
    var quotient = 10 / "5"; //returns 2
    var quotient = 10 / "coding"; //returns NaN
</script>

Although *NaN* represents invalid numbers, its data types is still *number*.

<script>
    typeof NaN; //returns number
</script>
--------------------------------------------------------------------


# THE *isNaN()* METHOD
The *isNaN()* method returns *true* if its arguement is not a legal number, otherwise *false*.

<script>
    var num1 = isNaN(5); //returns false
    var num2 = isNaN("5"); //returns false
    var num3 = isNaN("Making Progress"); //returns true
    var num4 = isNaN("five"); //returns true
</script>