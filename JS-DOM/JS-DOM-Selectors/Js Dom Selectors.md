# JAVASCRIPT DOM SELECTORS
With JavaScript, we can select any element from the DOM tree using the *document* object.

Why do we select element?

* To get their content

* To change their content

* To style them

* To get or change their attribute

* To remove them

* And many more...


# SELECT THE TOPMOST ELEMENTS
The topmost elements can be selected directly from the *document* object properties.

* *document.documentElement* selects <html>

* *document.head* selects <head>

* *document.body* selects <body>

HEAD OVER TO Topmost.html
---------------------------------------------------------------------


# SELECT AN ELEMENT BY ID
The *document.getElementById()* selects the element whose *id* attribute matches the specified string.

It is the best method to use when selecting a *single element*.

 <p id = "demo"> Lorem Ipsum. </p>
<script>
    document.getElementById("demo").innerHTML = "Making Progress";
</script>

=====================================================================


# SELECT ELEMENTS BY CLASS NAME
The *document.getElementsByClassName()* selects all elemens with the given class name.

It returns an array of objects. Why objects? Because in a DOM tree, all elements are objects.

In this example, we will select all elements with the *"big-green"* class name.

Then get access to each element using *for* loop.

HEAD OVER TO Classname.html

=====================================================================


# SELECT ELEMENTS BY TAG NAME
The *document.getElementsByTagName()* selects all elements with the given tag name.

It returns an array of objects.

In this example, we will style all <h3> elements.

HEAD OVER TO TagName.html

=====================================================================


# SELECT ELEMENTS BY NAME 
The *document.getElementByName()* selects all elements with the given name.

It returns an array of objects.

In this example, we use the *document.getElementsByName()* to select inputs by their *name* attributes.

Since it returns an array, we need to use the bracket notation ([0]) to select the first item of the array.

HEAD OVER To Name.html
---------------------------------------------------------------------


# SELECTING ELEMENTS USING CSS SELECTORS
The *document.querySelectorAll()* selects all elements that match the specified *selector*.

The selector must be a valid CSS selector.

It returns an array of the selected elements (nodes).

In this example, the element with the *demo* id is selected.

<p id = "demo">Lorem Ipsum </p>

<script>
    document.querySelectorAll("#demo")[0].innerHTML = "Making Progress";
</script>

In this example, all elements with the *big-green* class name are selected

HEAD OVER TO Selectors.html