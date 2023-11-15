# JAVASCRIPT *let* STATEMENT
The *let* statement declares variables that are limited to the scope of a block statement.

A *block statement* is a group of statements enclosed by curly brackets{}.

<script>
    {
        let myVar = "Making";
        //myVar can be used here
    }

    //myVar can NOT be used here
</script>


# SCOPING RULES
To better understand, let's compare *var* and *let* when they are used in a *function*.

The scope of a *var* variable is the *entire function*.

The scope of a *let* variable is the *block where it was defined*.

FOR EXAMPLE:

<script>
    function varTest(){
        var x = 4;
        {
            var x = 8; //same variable
            alert(x); //shows 8
        }
        alert(x); //shows 8
    }

    function letTest(){
        let x = 4; 
        {
            let x = 8; //same variable
            alert(x); //shows 8
        }
        alert(x); //shows 4
    }
</script>

Notice that *x* was redeclared by *var*.

On the other hand, *x* was NOT redeclared by *let*.

Instead, it created a new *x* variable that is only available to its block scope.
---------------------------------------------------------------------


# USING *let* IN A LOOP
Using *let* in a loop makes sure that you don't redeclare any variable outside the loop.

In this example, the *num* variable is redeclared.

<script>
    var num = 10;

    for(var num = 0; num < 15; num++){
        //block of codes
    }
    //num is 15 here
    document.getElementById("demo").innerHTML = num;
</script>

IN this example, the *num* variable is NOT redeclared

<script>
    var num = 10;
    
    for(let num = 0; num < 15; num++){
        //block of codes
    }
    // num is 10 here
    document.getElementById("demo").innerHTML = num;
</script>

*NOTE! Using *let* in loops is a good practice as it does not mess with your other variables.*
---------------------------------------------------------------------


# WINDOW OBJECT PROPERTIES FOR VARIABLES
The *var* statement creates a property for the *window* object.

The *window* object is a global object that contains the properties of the document.

In this example, the *animal* variable can be accessed using *window.animal*.

<script>
    var animal = "lion";
    document.getElementById("demo").innerHTML = window.animal;
</script>

HEAD OVER TO Window-var.html 

On the other hand, the *let* statement does NOT create a propert for the *window* object.

In this example below, *animal* variable can NOT be accessed using *window.animal*.

<script>
    let animal = "lion";
    document.getElementById("demo").innerHTML = window.animal;
</script>

HEAD OVER TO window-let.html 
---------------------------------------------------------------------


# *let* HOISITNG
Variables declared with the *let* statement are NOT hoisted to the top.

<script>
    animal = "lion";
    document.write(animal); // animal can NOT be used here
    let animal; //replace let with var to see the difference
</script>