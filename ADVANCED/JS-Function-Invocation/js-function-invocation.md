# JAVASCRIPT FUNCTION INVOCATION
You already know that *calling a function* will execute the codes inside it.

Calling a function can also be referred to as Invoking a function.

<script>
    function addNumbers(x, y){
        return x + y;
    }
    document.getElementById("demo").innerHTML = 
    addNumbers(5, 3); //invokes the function
</script>

====================================================================


# INVOKING FUNCTION WITH DEFAULT PARAMETERS
A function can have default parameters.

A function with default parameter can be invoked even if there is no argument is passed.

<script>
    function sayHello(message = "Making Progress"){
        alert(message);
    }
</script>

=====================================================================


# INVOKING FUNCTION WITH GLOBAL OBJECT
All functions declared in the global scope are added to the *global object*.

The *window* object represents the global object.

<script>
    function addNumbers(x, y){
        return x + y;
    }
    document.getElementById("demo").innerHTML = 
    window.addNumbers(5, 3); //invokes the function using window object
</script>


=====================================================================


# INVOKING FUNCTION IN AN OBJECT
The *this* keyword inside a function in an *object* referers to the *object* itself.

<script>
    var animal = {
        name: "Tiger",
        type: "Cat",
        showInfo: function(){
            return "The " + this.name + " is " + this.type;
        }
    }

    document.getElementById("demo").innerHTML = 
    animal.showInfo(); //invokes the function inside the object
</script>