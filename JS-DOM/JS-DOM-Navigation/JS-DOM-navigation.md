# JS NAVIGATING NODES
*Navigating nodes* means reaching nodes in the DOM tree.

The following *document* object properties are used to navigate nodes:

* *parentNode*

* *firstChild*

* *lastChid*

* *childNodes[index]

* *previousSibling*

*  *nextSibling*

The properties mentioned above will navigate not just element nodes, but also *text* and *comment* nodes.

Commonly, we only need to navigate *element nodes* for efficiency.


# NAVIGATING ELEMENT NODES
The following *document* object properties are used to navigate *element nodes*:

* *parentElement*

* *firstElementChild*

* lastElementChild*

* children[index]*

* previousElementSibling*

* nextElementSibling*

# PARENT AND CHILDREN

The *parentElement* property returns the DOM node's parent element.

In this example, we will select the <p> element's parent element which is the <div>.

Then we will change it's background color using the *style.background* property.

*HEAD OVER TO parent.html*

The *firstElementChild* property returns the DOM node's first child element.

In this example, we will select the first child element of the <div> element

*HEAD OVER TO FirstElement.html*


The *lastChildElement* property returns the DOM node's last child element.

In this example, we will select the last child element of the <div> element

*HEAD OVER TO LastElement.html*

The *children* property retuns a collection of the selected element's children.

The collection is like an *array*, therefore, we can access each item using bracket notation.

Remember, in bracket notation, the first item is 0.

In this example, we will select and style the *<div>* element's *second child*

*HEAD OVER TO children.html*


# SIBLINGS
The *previousElementSibling* returns the previous element prior to the specified one in a parent's children list.

In this example, we will select the <p> element.

Then we will select and style the element that comes before it: the <h1> element.

*HEAD OVER TO siblings.html*


The *nextElementSibling* returns the next element prior to the specified one in a parent's children list.

In this example, we will select the <p> element.

Then we will select and style the element that comes after it: the <a> element.

*HEAD OVER TO Next-sibling.html*