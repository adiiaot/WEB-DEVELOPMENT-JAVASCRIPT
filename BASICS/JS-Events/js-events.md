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


# THE *mouseover* EVENT
The *mouseover* event fires at an element when a mouse is moved onto the element.

<script>
    var elem = document.getElementById("demo");

    elem.addEventListener("mouseover", function(){
        elem.innerHTML = "Making progress";
    });
</script>

HEAD OVER TO Using-mouseover-Event.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *keypress* EVENT
The *keypress* event fires when a key is pressed.

<script>
    var area = document.getElementById("area");

    area.addEventListener("keypress", function(){
        document.getElementById("demo").innerHTML = area;
    });
</script>

HEAD OVER TO Using-keypress-Event.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *focus* EVENT
The *focus* event fires when an element is *focused*.

In the example below, when the textarea is focused, its *background color* changes

<script>
    var area = document.getElementById("area");

    area.addEventListener("focus", function(){
        area.style.background = "yellow";
    });
</script>

HEAD OVER TO Using-focus-Event.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *blur* EVENT
The *blur* event fires when an element has *lost focus*.

In the example below, when the textarea is focused, background color changes.

When it loses focus, background color becomes white again.

<script>
    var area = document.getElementById("area");

    area.addEventListener("focus", function(){
        area.style.background = "yellow";
    });

    area.addEventListener("blur", function(){
        area.style.background = "white";
    });
</script>

HEAD OVER TO Using-blur-Event.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *resize* EVENT
The *resize* event fires when the window is resized.

<script>
    window.addEventListener("resize", function(){
        document.getElementById("windowWidth").innerHTML = window.innerWidth;
        document.getElementById("windowHeight").innerHTML = window.innerHeight;
    });
</script>

HEAD OVER TO Using-resize-event.html TO SEE THE OUTPUT OF THIS CODE