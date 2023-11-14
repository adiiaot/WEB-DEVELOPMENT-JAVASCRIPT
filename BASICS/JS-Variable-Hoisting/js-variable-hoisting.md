# JAVASCRIPT VARIABLE HOISTING
In JavaScript, *Hoisting* is the default behaviour of declaring any variables to the top.

Variable declarations are always executed first before any code is executed in the current scope.

For example:

<script>
    animal = "Lion";
    document.getElementById("demo").innerHTML = animal;
    var animal;
</script>

Although the *var* animal declaration is at the bottom of the code, it is still going to be executed first. 

This behaviour is called *hoisting*.

The example below is equivalent to this;

<script>
    var animal;
    animal = "Lion";
    document.getElementById("demo").innerHTML = animal;
</script>


# VARIABLE INITIALIZATIONS ARE NOT HOISTED
In JavaScript, variable initialization are not hoisted, only declarations are hoisted.

*Note! when you assign a value to a variable, it is called initialization.*

This example below, will work as expected because the *animal* was initialized first before being used:

<script>
    var animal;
    animal = "Lion";
    document.getElementById("demo").innerHTML = animal;
</script>

The example below, will not WORK as expected because the *animal* was used first before being initialized.

<script>
    var animal;
    document.getElementById("demo").innerHTML = animal;
    animal = "Lion";
</script>
---------------------------------------------------------------------

# RECOMMENDED: DECLARE VARIABLES AT THE TOP
Although hoisting is a good feature of JavaScript, it is still recommended to declare your variables at the *top of the scope*.

This will maintain the readability of your code and can avoid errors.