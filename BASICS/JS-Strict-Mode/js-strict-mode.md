# JAVASCRIPT STRICT MODE
JavaScript's *strict mode* was introduced in ECMAScript 5.

# INVOKING STRICT MODE
To invoke or to start using strict mode, put the exact statement "Use strict" at the top of the script.

<script>
    "use strict"
    var text = "This variable is in a strict mode script!";
</script>

To invoke strict mode in a *function*, put the "use strict" at top of the bottom.

<script>
    function myFunc(){
        "use strict";
        var text = "This variable is in a strict mode script!";
        alert(text);
    }
</script>

In this section, we will study the effects of strict mode to variables.

# VARIABLES IN STRICT MODE
Undeclared variables in strict mode will cause an error.

<script>
    "use strict";
    animal = "Lion"; //initialized but not declared
    document.write(animal);
</script>

HEAD OVER TO Error-report.html TO SEE THE OUTPUT IN THE DEVELOPER CONSOLE

The *error report* can be seen by using a desktop/laptop browser's developer console.

The developer console can be accessed by pressing the F12 key.

However, we can also see the error on a mobile device, try using the *try...catch* statement

<script>
    "use strict"
    try{
        animal = "Lion";
        document.write(animal);
    }
    catch (err){
        document.write(err);
    }
</script>

HEAD OVER TO Mobile-report.html 

Undeclared variables in a strict mode function will only cause error in that function's scope, not outside:

<script>
    myVariale = "Making Progress"; // does not cause an error

    function myFunc(){
        "use strict";
        animal = "Lion";
        alert(animal);
    }
</script>

We can see the error by calling *myFunc()* function inside the *try...catch* statement

<script>
    try{
        myFunc();
    }
    catch(err){
        document.write(err);
    }
</script>

HEAD OVER TO Function-error.html
---------------------------------------------------------------------


# OTHER STRICT MODE RESTRICTIONS
Strict mode requires function parameter names be unique.

The example below will throw a syntax error.

<script>
    function (x, x, y){ //syntax error
        "use strict";
        alert(x + x + y);
    }
</script>

In strict mode, a leading *zero* will cause an error.

The example below will throw a *syntax error*.

<script>
    "use strict";
    var sum = 02 + 3;
    alert(sum);
</script>