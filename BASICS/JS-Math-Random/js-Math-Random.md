# JAVASCRIPT MATH RANDOM
In this section, you will learn how to generate a random number.

# THE *random()* METHOD
The *Math.random()* method returns a random floating point (number with decimals) between 0 (included) and 1 (excluded).

<script>
    var random = Math.random();
</script>

HEAD OVER TO Random.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# GET RANDOM INTEGER BETWEEN TWO NUMBERS
The example above only gets a random *floating point* (number with decimals) between 0 and 1.

What if we need to get a random *integer* between two specified integers? Here's how:

<script>
    //minimum is included, maximum is excluded
    function getRandomInt(min, max){
        return Math.floor(Math.random() * (max - min)) + min;
    }
</script>

HEAD OVER TO Random-Number.html TO SEE THE OUTPUT OF THIS CODE
========

To get a random number that also includes the maximum number, use this function:


<script>
    //minimum is included, maximum is excluded
    function getRandomInt(min, max){
        return Math.floor(Math.random() * (max - min + 1)) + min;
    }
</script>