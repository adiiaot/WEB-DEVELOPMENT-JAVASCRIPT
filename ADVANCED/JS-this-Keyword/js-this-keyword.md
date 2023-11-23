# JAVASCRIPT *this* KEYWORD
The *this* keyword represents the object where it belongs to.

In this example, the *this* keyword inside the *animal* object represents the *animal* object itself.

<script>
    const animal = {
        name: "lion", 
        color: "yellow",
        isWild: true,
        showAnimal: function(){
            document.getElementById("demo").innerHTML = "The " + this.name + " is " + this.color;
        }
    };

    animal.showAnimal();
</script>

HEAD OVER TO This.html

Notice that the *this* keyword is used inside the *showAnimal* method, and the *showAnimal* method belongs to the *animal* object.

Therefore, the *this* keyword represents the *animal* object.
---------------------------------------------------------------------


# THE GLOBAL OBJECT
The *global object* always exists in the global scope.

The *window* object represents the *global object*.

It contains properties like the *window.document* property.

<script>
    window.document.write("Making Progress");
</script>

It also contains methods like the *window.alert()* method

<script>
    window.alert("Making Progress");
</script>

====================
====================

The *window* object also contains the VARIABLES that were declared using the *var* keyword and the FUNCTIONS that you declare in the *global scope*.

<script>
    var animal = "lion";
    function greetUser(){
        alert("Making Progress!");
    }
</script>


Both the function and the variable above can be accessed using the *window* object.

<script>
    var animal = "lion";
    function greetUser(){
        alert("Making Progress!");
    }

    document.getElementById("demo").innerHTML = window.animal;
    window.greetUser();
</script>


HEAD OVER TO Global-scope.html
---------------------------------------------------------------------


# *this* IN A FUNCTION
The *this* keyword inside a function represents the *global object*

<script>
    var animal = "dog";
    function myFunc(){
        var x = this;
        x.alert("I want to buy a " + x.animal);
    }
</script>

HEAD OVER TO this-function.html
---------------------------------------------------------------------


# *this* ALONE
When *this* is used in the global scope alone, it represent the global object.

<script>
    this.alert("Making Progress");
</script>

---------------------------------------------------------------------


# *this* IN AN EVENT HANDLER
When *this* is used in an event handler, it represents the HTML element that received the event.

In the example, *this* represents the button clicked.

<script>
    const btn = document.getElementById("btn");

    btn.onclick = function(){
        this.style.background = "red";
        this.style.color = "white";
    };
</script>


HEAD OVER TO this-event.html