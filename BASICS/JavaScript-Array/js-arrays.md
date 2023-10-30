# JAVASCRIPT ARRAYS
JavaScript *arrays* are list-like objects.

A single array can store multiple data.

<script>
    var fruits = ["Lion", "Tiger", "Cheetah"];
</script>

In the code snippet above, one variable holds three values. 

This is what makes arrays special, it can hold many values.

Instead of storing multiple data like this:

<script>
    var person1 = "Roman";
    var person2 = "Ayo";
    var person3 = "Oluwadare";
    var person4 = "Adii";
</script>

We can just store multiple data like this:

<script>
    var persons = ["Roman", "Ayo", "Oluwadare", "Adii"];
</script>

Much efficient, right?
---------------------------------------------------------------------

# CREATING AN ARRAY
Arrays are created with square brackets [] and data are separated with commans (,).

<script>
    var animals = new Array("Lion", "Tiger", "Cheetah");
</script>

*Note: It is recommended to use square brackets as it's much faster in execution and more readable.*
---------------------------------------------------------------------


# ACCESS AN ARRAY ITEM
Array items are accessed using *integers*.

Arrays are *zero-indexed*

This means that count starts from 0, not from 1.

<script>
    var animals = ["Lion", "Tiger", "Cheetah"];
    document.getElementById("demo").innnerHTML = animals[0]; //prints out "Lion"
</script>

Notice that *animals[0]* returned the first element, which is *lion*.
---------------------------------------------------------------------


# ADD ITEMS TO AN ARRAY
* The *push()* method adds one or more elements (items) to the end of an array.

Here's an example of adding a single element:

<script>
    var animals = ["lion", "tiger", "cheetah"];
    animals.push("leopard");
</script>

* Adding Multiple elements:

<script>
    var animals = ["lion", "tiger", "cheetah"];
    animals.push("leopard", "giraffe", "zebra");
</script>

HEAD OVER TO *Add-Items-to-Arrays - Using-Push-Method (push-method.html)* TO SEE HOW I'VE ORGANIZED THE CODE TO OUTPUT THE THREE ELEMENTS
-------------
-------------

* The *unshift()* method adds one or more elements (items) to the FRONT of an array.

Here's an example of adding a single element to the front of the array.

<script>
    var animals = ["lion", "tiger", "cheetah"];
    animals.unshift("leopard");
</script>

* Adding multiple elements

<script>
      var animals = ["lion", "tiger", "cheetah"];
    animals.unshift("leopard", "zebra", "dog");
</script>

HEAD OVER TO *Add-Items-to-Arrays - Using-unshift-Method (unshift-method.html)* TO SEE HOW I'VE ORGANIZED THE CODE TO OUTPUT THE THREE ELEMENTS
---------------------------------------------------------------------


# REMOVE ITEMS FROM AN ARRAY
* The *pop()* method removes the LAST ELEMENT of an array.

<script>
    var animals = ["Lion", "Tiger", "Jaguar", "Panther", "Zebra"];
    animals.pop(); //removes "Zebra", personally I see them as weak!
</script>

HEAD OVER TO Remove-items-From-Array - Using-Pop-method (pop.html) TO SEE THE OUTPUT OF THIS CODE
---------------
---------------

* The *shift()* method removes the FIRST ELEMENT of an array.

<script>
    var animals = ["Lion", "Tiger", "Jaguar", "Panther"];
    animals.shift(); //removes "Lion"
</script>

HEAD OVER TO Remove-items-From-Array - Using-Shift-method (shift.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------



# GET THE LENGTH OF AN ARRAY
The *length* of an array represents its number of elements.

The *length* property returns the number of elements of an array.

<script>
    var animals = ["Lion", "Tiger", "Jaguar", "Panther"];
    document.getElementById("demo").innerHTML = animals.length;
</script>

HEAD OVER TO Getting-Length-Of-Array (length.html) TO SEE THE OUTPUT
---------------------------------------------------------------------



# ACCESS THE LAST ITEM
To access the last item of an array, deduct 1 from its *length*.

<script>
    var animals = ["Lion", "Tiger", "Jaguar", "Panther"];
    var lastItem = animals[animals.length -1];

    document.getElementById("demo").innerHTML = lastItem
</script>

HEAD OVER TO Accessing-Last-Item (access-lastitem.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# LOOP OVER AN ARRAY
Looping over an array means accessing its data individually.

We can use the *for* loop to loop over an array.

<script>
    var animals = ["Lion", "Tiger", "Cheetah", "Zebra"];

    for(var i = 0; i < animals.length; i++){
        document.getElementById("demo").innerHTML += animals
    }
</script>

HEAD OVER TO Loop-over-an-Array (loop-Array.html) TO SEE THE OUTPUT OF THIS CODE

* Notice that we used the *addition assignment (+=)* operator with the *innerHTML* property.

This makes sure that the printed elements do not get overwritten.

*YOU WILL LEARN ABOUT JAVASCRIPT LOOPS LATER ON IN THIS COURSE*
--------------------------------------------------------------------



# ARRAYS ARE OBJECTS
The data type of an array is *object*.

This can be shown using the *typeof* operator.

<script>
    var animals = ["lion", "tiger", "cheetah", "zebra"];
    var type = typeof animals; //returns objects

    document.getElementById("demo").innerHTML = type;
</script>