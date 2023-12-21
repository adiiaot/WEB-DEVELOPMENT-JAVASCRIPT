# JAVASCRIPT DOM EVENTS
With JavaScript and DOM, we can listen to events that happen to elements.

For example, we can *listen* then *do something* when a button is clicked.

# THE *addEventListener()* METHOD
The *addEventListener()* method sets up a function that will be called whenever the specified event is fired to the element.

Syntax:

element.addEventListener(eventType, listenerFunction)

1. eventType - a string representing the event type.

2. listenerFunction - a listener function, it will be called when the event fires.


# CLICK EVENT 
In this example, when the button is clicked, a pop-up dialog will be shown.

HEAD OVER TO Click-Event.html
---------------------------------------------------------------------

# LOAD EVENT
In this example, when the image file is loaded, a pop-up dialog will be shown.

HEAD OVER TO Load-Event.html
---------------------------------------------------------------------

# CHANGE EVENT
In this example, every time the value of the <input> changes, we will get its value and write it to a <p> element.


HEAD OVER TO Change-Event.html