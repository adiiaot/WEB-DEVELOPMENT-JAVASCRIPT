# JAVASCRIPT VARIABLE SCOPE
The accessibility of variables is defined by their *scope*. 

In JavaScript, there are 2 variable scopes:

* Global Scope
* Local Scope

# GLOBAL VARIABLES
Any *variable* that is declared *outside* a function has a *global scope*.

A global variable can be accessed by all *functions* and scripts in a document

<script>
    var animal = "Lion";
    //animal can be used here

    function myFunc(){
        //animal can be used here
        alert(animal);
    }
</script>

Also, any variable that is *initialized* or has been assigned a value *inside a function* without being declared first will be *global*. 

For example

<script>
    myFunc(); //call the function first

    //animal can be used here
    document.getElementById("demo").innerHTML = "I love " + animal;

    function myFunc(){
        animal = "Lion";
        alert(animal);
    }
</script>
HEAD OVER TO Global-Scope.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# LOCAL VARIABLES
Any variable that is declared inside a function has a local scope.

A local variable can be only accessed by the function where it was declared.

<script>
    // animal can not be used here
    document.getElementById("demo").innerHTML = animal;

    function myFunc(){
        var animal = "Lion";
        alert(animal);
    }
</script>
HEAD OVER TO Local-Scope.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# JAVASCRIPT FUNCTIONS
*Functions* are also *variables*, therefore the rules mentioned above also apply to functions.

A *global function*:

<script>
    function myFunc() {
        document.getElementById("demo").innerHTML = "Making";
    }

    // myFunc() can be used here

    function myFunc2() {
        //myFunc() can be used here
        myFunc();
        document.getElementById("demo").innerHTML += "Progress";
    }
</script>

HEAD OVER TO Global-function.html
=============
=============

A *local function*:

<script>
    //getSum() can NOT be used here

    function myFunc2(){
        function getSum(x, y){
            return x + y;
        }

        // getSum() can be used here
        document.getElementById("demo").innerHTML = "the sum of 5 and 3 is " + getSum(5, 3);
    }
</script>

HEAD OVER TO Local-Function.html 