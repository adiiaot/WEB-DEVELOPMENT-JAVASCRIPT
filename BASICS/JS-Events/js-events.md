# JAVASCRIPT EVENTS
Events are *actions* that happen in the system you are programming.

The system fires a signal when events happen, so we can do something when they do.

For example, we can perform a task when a *button is clicked*.

<script>
    var btn = document.getElementById("btn");

    //the block of code below is called event handler
    btn.onclick = function(){
        alert("The button was clicked, and the task is to show this dialog box.");
    }
</script>

The block of code that executes when an event fires is called *event handler*.

It is also called *event listener*.
---------------------------------------------------------------------


# INLINE EVENT HANDLERS
We can also write event handlers inside an HTML element.

This can be done using *event handler attributes*.


<button onclick = 'alert("The button is clicked, and the task is to show this dialog box")'>Click Me </button>

<script>
    function myFunc(){
        alert("Making Progress");
    }
</script>
---------------------------------------------------------------------


# THE *addEventListener()* METHOD
The *addEventListener()* method sets up a *function* that will be called when an event happens.

*Syntax*:
<script>
    element.addEventListener(eventType, listenerFunction)
</script>

1. *eventType* - a string representing the event type
2. *listenerFunction* - a listener function, it will be called when the event fires.

Here's an example:

<script>
    var btn = document.getElementById("btn");

    btn.addEventListener("click", function(){
        alert("The button was clicked, and the task is to show this dialog box");
    })
</script>
---------------------------------------------------------------------

## MORE EVENT TYPES
In JavaScript, there are many *event types*. Here are some of the most useful:

# THE *change* EVENT
The *change* event fires when the values of the *<input>*, *<select>* and *<textarea>* elements change.

The example below gets the value of the *<select>* element when a value is selected.

<script>
    var select = document.getElementById("city");

    select.addEventListener("change", function(){
        var val = document.getElementById("city").value;

        document.getElementById("demo").innerHTML = val;
    });
</script>

HEAD OVER TO Using-change-Event.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------