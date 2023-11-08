# JAVASCRIPT *for...of* LOOP
The *for...of* statement loops over *iterable objects*.

The most basic *iterable objects are *arrays* and *strings*.

Syntax:

<script>
    for(variable of iterable){
        // statements or code blocks
    }
</script>

* *variable* - on each iteration the value of the property is assigned to *variable*

* *iterable* - the *iterable object* being iterated over (no be lie!)

Here's an example of looping through the values of an *array*.

<script>
    var animals = ["lion", "tiger",  "dog"];

    for(value of animals){
        document.write(value + "<br>");
    }
</script>

HEAD OVER TO Looping-Array.html TO SEE THE OUTPUT OF THIS CODE
===========
===========

Here's an example of looping over a *string*.

<script>
    var text = "Adiidevs";

    for (letter of text){
        document.write(letter + "<br>");
    }
</script>

HEAD OVER TO Looping-Strings.html TO SEE THE OUTPUT OF THIS CODE