# JAVASCRIPT *if...else* STATEMENT
In this section, we will study about *conditional statements*.

Conditional Statements are used to execute code based on different conditions.

# THE *if* STATEMENT
The *if* statement executes a block of codes if the given condition is *true*.

Syntax:

<script>
    if(condition){
        // block of codes to be executed when the condtion is true
    }
</script>

In the example below, if the age is *more than* 18, a pop-up dialog will be shown.

<script>
    var age = 23;
    if (age > 18){
        alert("User is old enough to enter");
    }
</script>
HEAD OVER TO if-statement.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *if...else* STATEMENT
The *else* statement executes a block of codes when the given condition is *false*.

Syntax:

<script>
    if(condition){
        //block of code to be executed if condition is true
    }else {
        //block of codes to be executed if condition is false
    }
</script>

Here's an example below,

<script>
    var age = 14;
    if (age > 18){
        alert("User is old enough to enter");
    } else {
        alert("User is still young, LEAVE!");
    }
</script>

HEAD OVER TO if-else-Statement.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


Here's is an illustrative example, the user will be asked to enter their age.

If they are above *18*, they will be allowed to enter.

If they are below *18*, they will NOT be allowed to enter.

<script>
    document.getElementById("submit").addEventListener("click", function(){
        var age = document.getElementById("age").value;
        if (age > 18){
            alert("User is old enough to enter");
        } else {
            alert("User is still young, My friend LEAVE!");
        }
    });
</script>

HEAD OVER TO Sample.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *else...if* STATEMENT
The *else if* statement executes a block of codes if its specified condtion is *true* and the FIRST CONDITION is *false*.

Syntax:

<script>
    if(condition){
        //block of codes to be executed when condition is true
    } else if{
        //block of codes to be executed when condition is false
    } else {
        //block of codes to be executed when condition1 and condition2 are false
    }
</script>

Here's a basic example:

<script>
    var x = 15;

    if(x < 10){
        document.getElementById("demo").innerHTML = "x is less than 10";
    } else if {
        document.getElementById("demo").innerHTML = "x is more than 10";
    } else {
        document.getElementById("demo").innerHTML = "x is 10 because it's neither less than or more than 10";
    }
</script>

HEAD OVER TO else-if-Statement.html TO SEE THE OUTPUT OF THIS CODE 
---------------------------------------------------------------------


The example below, greets the user depending of the current time of the day.

If the time is below 11:00, it says, "Good morning".

If the time is below 18:00, it says, "Good day".

Otherwise, "Good evening".

<script>
    function greetUser(){
        var time = new Date().getHours();
        if (time < 11){
            return "Good Morning";
        } else if (time < 18){
            return "Good day";
        } else {
            return "Good evening";
        }
    }

    document.getElementById("demo").innerHTML = greetUser();
</script>

HEAD OVER TO Sample2.html TO SEE THE OUTPUT OF THIS CODE