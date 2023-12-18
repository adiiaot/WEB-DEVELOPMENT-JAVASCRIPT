# JS DOM CSS OR STYLING
With JavaScript and DOM, we can style HTML elements.

In CSS, as you already know, styling elements means changing their properties.

It's the same with JavaScript.

# STYLING ELEMENTS WITH DOM
To change the styles of an element, use the *style* object of a node.

Here is the syntax:

node.style.property = "value";

# EXAMPLE
In this example, we will change the *color* property of <p> element.

<script>
    document.getElementById("demo").style.color = "green";
</script>


# HIDING AND SHOWING AN ELEMENT
To hide and show an element, set the *display* property to *none* and *block* respectively.

HEAD OVER TO Hide-Show.html
---------------------------------------------------------------------


# WHAT ABOUT PROPERTIES WITH HYPEN?
Properties with hypen like *font-size*, *text-decoration* and *background-color* should be written in camel-case.

For example:

* font-size = fontSize
* text-decoration = textDecoration
* background-color = backgroundColor

<script>
    const element = document.getElementById("demo");

    element.style.fontSize = "18px";
    element.style.textDecoration = "none";
    element.style.backgroundColor = "green";
</script>