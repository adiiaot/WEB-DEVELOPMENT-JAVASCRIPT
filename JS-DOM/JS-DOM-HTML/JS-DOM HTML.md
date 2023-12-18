# JAVASCRIPT DOM HTML
In this section, we will study about the amazing things that we can do to HTML using the DOM.

# GETTING ELEMENT'S CONTENT
The *innerHTML* property returns the content of an HTML element.

<script>
    const list = document.getElementById("list");
    alert(list.innerHTML);
</script>

HEAD OVER TO InnerHTML.html
---------------------------------------------------------------------


# REPLACING ELEMENT'S CONTENT
The *innerHTML* property can also be used to replace the content of an HTML element.

HEAD OVER TO Replace.html
---------------------------------------------------------------------

Note! The *innerHTML* simply adds content to the selected element if it's empty.


# CREATING ELEMENTS (NODES)
Before we can insert elements (nodes) to the DOM, we should first learn how to create them in JavaScript.

To create an element, use the *document.createElement(element)* method.

The code below creates a paragraph <p> element:

<script>
    const element = document.createElement("p");
</script>

Of course, we want to add text inside the <p> element.

To do this, we need to create a *text node* and insert the text node to the <p> element.

<script>
    element.appendChild(textNode);
</script>

Finally, we have successfully created a <p> element with a text inside it.

Now, we can insert the created element to another parent element by using again, the *appendChild()* method.

HEAD OVER TO Creating-Elements.html
---------------------------------------------------------------------


# INSERTING TO ELEMENTS
Commonly, we only want to insert to elements not completely replace its content.

The *ParentNode.prepend()* method inserts an element (node) *before the first child* of the *ParentNode*.

HEAD OVER TO Inserting-Elements.html

The *ParentNode.append()* method inserts an element (node) *after the last child* of the *ParentNode*.

HEAD OVER TO Inserting2.html
---------------------------------------------------------------------


# REMOVING ELEMENTS
To remove an element, use the *node.remove()* method.

The *node.remove()* method removes the *node* from the tree it belongs to.

HEAD OVER TO Removing-Element.html
---------------------------------------------------------------------


# WORKING WITH ATTRIBUTES 
With JavaScript and DOM, we can get, set, and change an attribute's value.

# GETTING ATTRIBUTE VALUE
The *node.getAttribute(attributeName)* returns the value of the specified attribute.

In this example, we will get the value of the *href* attribute.

<script>
    <a href = "https://www.example.com" id = "demo">Go To example.com</a>
</script>

HEAD OVER TO Getting-Attribute.html
---------------------------------------------------------------------


# SETTING OR CHANGING ATTRIBUTE VALUE
The *node.setAttribute(attibuteName, value)* sets the value of an attribute on the speciifed element.

If the attribute already exists, the value is changed.

In this example, we will *set* the *src* attribute of the <img> element.

HEAD OVER TO Set-Attribute.html

In the next example, we will *change* the *src* attribute of the <img> element.

HEAD OVER TO Change-Attribute.html