# JAVASCRIPT TIMEOUT AND INTERVAL
JavaScript allows us to execute codes at specified *time intervals*.

This is useful when you want to delay executing a piece of code or repeatedly run the same code.

# JAVASCRIPT TIMEOUT
The *setTimeout()* method sets a timer which executes a function once the timer expires.

Syntax:

<script>
    var timeoutId = setTimeout(function(){
        //codes
    }, delay);
</script>

* *function* - will be executed when the timer expires
* *delay* - the time in milliseconds, the timer should wait before executing the *function*

In the example below, a pop-up dialog will be shown after 3 seconds (3000 milliseconds).

<script>
    var myTimeout = setTimeout(function(){
        alert("You are making Progress!");
    }, 3000);
</script>

HEAD OVER TO Timeout.html TO SEE THE OUTPUT OF THIS CODE

You can also separate the function:

<script>
    function myFunc(){
        alert("You are making progress!");
    }

    var myTimeout = setTimeout(myFunc, 3000);
</script>

HEAD OVER TO Timeout2.html TO SEE THE OUTPUT OF THIS CODE
--------------------------------------------------------------------


# CANCELING A TIMEOUT
The *clearTimeout()* method cancels a timeout function specified by the *setTimeout()* method.

Simply specify the *timeoutID* of the timeout you want to cancel.

In the example below, *myTimeout* will be canceled when you press the button.

<script>
    var myTimeout = setTimeout(function(){
        alert("Making Progress!");
    }, 3000);

    function cancelTimeout(){
        clearTimeout(myTimeout);
    }
</script>

HEAD OVER TO Cancel-timeout.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# JAVASCRIPT INTERVAL
The *setInterval* method repeatedly calls a function 

Syntax:

<script>
    var intervalID = setInterval(function(){
        // codes
    }, delay);
</script>

* *function* - will be executed every *delay* milliseconds 
* *delay* - the time in milliseconds, the timer should delay in between the execution of the *function*.

In the example, 10 will be added to x every *1 second (1000 milliseconds)*

<script>
    var x = 10;

    function myFunc() {
        // adds x to 10
        x += 10;
        document.getElementById("demo").innerHTML = x;
    }

    var myInterval = setInterval(myFunc, 1000);
</script>

HEAD OVER TO Interval.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# STOPPING AN INTERVAL
The *clearInterval()* method stops a timed function specified by the *setInterval()* method.

Simply specify the *intervalID* of the interval you want to stop.

In the example below, myInterval will be stopped when you press the button, heck we can even try to calculate our money!.

WATCH

<script>
    var x = 10;

    function myFunc() {
        x += 10;

        document.getElementById("demo").innerHTML = x;
    }

    var myInterval = setInterval(myFunc, 1000);

    function cancelInterval() {
        clearInterval(myInterval);
    }
</script>

HEAD OVER TO Cancel-Interval.html TO SEE THE OUTPUT OF THIS CODE