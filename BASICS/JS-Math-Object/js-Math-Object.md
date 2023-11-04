# JAVASCRIPT MATH OBJECT
The *Math* object is a built-in JavaScript object.

The *Math* object contains properties and methods that allow us to do mathematical tasks.

# THE *ceil()* METHOD
The *Math.ceil()* method rounds up a number to the nearest whole number or integer.

<script>
    var num1 = Math.ceil(.90); //returns 1
    var num2 = Math.ceil(1.70); //returns 2
    var num3 = Math.ceil(21.60); //returns 22
</script>

HEAD OVER TO The-ceil-Method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *floor()* METHOD
The *Math.floor()* method *rounds down* a number to the nearest whole number or integer.

<script>
    var num1 = Math.floor(1.10); //returns 1
    var num2 = Math.floor(3.21); //returns 3
    var num3 = Math.floor(21.30); //returns 21
</script>

HEAD OVER TO The-floor-Method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *round()* METHOD
The *Math.round()* method *rounds* a number to the nearest whole numberr or integer.

<script>
    var num1 = Math.round(1.10); //returns 1
    var num2 = Math.round(1.70); //returns 2
    var num3 = Math.round(21.50); //returns 22
    var num4 = Math.round(-7.34); //returns -7
</script>

HEAD OVER TO The-round-Method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *sqrt()* METHOD
The *Math.sqrt()* method returns the *square root* of a number.

<script>
    var num1 = Math.sqrt(4); //returns 2
    var num2 = Math.sqrt(100);  //returns 10
    var num3 = Math.sqrt(3.21); //returns 1.7916472867168918
    var num4 = Math.sqrt(-9);  //returns NaN
</script>

It returns *NaN* when the given number is *negative*

HEAD OVER TO The-sqrt-Method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *cbrt()* METHOD
The *Math.cbrt()* method returns the *cube root* of a number.

<script>
    var num1 = Math.cbrt(8); //returns 4
    var num2 = Math.cbrt(100); //returns 4.641588833612779
    var num3 = Math.cbrt(3.21); //returns 1.4751460163788064
    var num4 = Math.cbrt(-27); //returns -3
</script>

HEAD OVER TO The-cbrt-Method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *abs()* METHOD
The *Math.abs()* method returns the *absolute value* of a number.

<script>
    var num1 = Math.abs(5); //returns 5
    var num2 = Math.abs(-5); //returns 5
    var num3 = Math.abs(3.21); //returns 3.21
    var num4 = Math.abs(-3.21); //returns 3.21
</script>

HEAD OVER TO The-abs-Method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *max()* METHOD
The *Math.max()* method returns the *largest number* from a given *array* of numbers.

<script>
    var num1 = Math.max(1, 2, 3); //returns 3
    var num2 = Math.max(-1, -2, -3); //returns -1
</script>

HEAD OVER TO The-max-method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *min()* METHOD
The *Math.min()* method returns the *smallest number from a given *array* of numbers. 

<script>
    var num1 = Math.min(1, 2, 3); //returns 1
    var num2 = Math.min(-1, -2, -3); //returns -3
</script>

HEAD OVER TO The-min-method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *pow()* METHOD
The *Math.pow()* method returns the base to the exponent power.

It takes 2 arguments: Base, exponent.

In the example below, 2 is raised to the power of 3. That is, 

2 * 2 * 2 = 8.

<script>
    var num1 = Math.pow(2, 3); //returns 8
</script>

HEAD OVER TO The-pow-Method.html TO SEE THE OUTPUT OF THIS CODE