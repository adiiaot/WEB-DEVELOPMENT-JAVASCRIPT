# DOM NODES
In a DOM tree, every element is an object.

For example, the *document.body* object represents the *<body>* element.

# WHAT IS A NODE?
A node is any *object* in the DOM tree.

Therefore, a node can be any HTML elements such as <html>, <body>, <head> and all the other elements.

# NODE RELATIONSHIPS
The nodes in the DOM tree have relationships with each other.
 
We use the terms *parent*, *child* and *sibling* to describe their relationships.

Let's take a look at our DOM tree explanations:

* <html> is the root or top node meaning it has no parents

* <html> is the parent of <head> and <body>

* <head> is the first child of <html>

* <body> is the last child of <html>

* <head> has one child: <title>

* <body> has two children: <h1> and <p>

* <h1> is the first child of <body>

* <p> is the last child of <body>

* <head> and <body> are siblings

* <h1> and <p> are siblings.

Even the text inside the elements are considered as nodes, they are called *text nodes*.

Therefore:

* "The Title" is a child of <title>

* "A Header" is a child of <h1>

* "A Paragraph" is a child of <p>

# EVERYTHING IS A NODE
In a Document Object Model tree, everything is a node.

As you know, elements are nodes.

Additionally, *text*, *attributes* and even *comments* are considered as *nodes*.