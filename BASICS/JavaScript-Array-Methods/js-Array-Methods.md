# JAVASCRIP ARRAY METHODS
In this section, we will study the most useful *Array* methods.

# THE *forEach()* METHOD
The *forEach()* method is another way to loop over an array, or access each element's data.

It executes a *callback function* for each array element.

<script>
    var animals = ["Lion", "Tiger", "Dog"];

    animals.forEach(function (val, i, arr){
        document.write(i + ": " + val + "<br>");
    });
</script>
==========
HEAD OVER TO forEach-Method (forEach.html) TO SEE THE OUTPUT

The callback function is invoked with 3 arguments.

1. The *value* of the element.
2. The *index* of the element.
3. The *array* itself.

---------------------------------------------------------------------

# ARRAY TO STRINGS
The *join()* method creates and returns a new string by combining all the elements.

The elements are separated by the specified separator character.

If none is specified, it separates the elements with commas.

<script>
    var animals = ["lion", "tiger", "dog"];
    var str = animals.join();
    document.write(str);
</script>

HEAD OVER TO Array-To-Strings (Using-Join-Method.html) TO SEE THE OUTPUT
======
=====

Here's an example with specified separator:

<script>
    var animals = ["lion", "tiger", "dog"];
    var str = animals.join("-");
    document.write(str);
</script>

TRY THIS ONE OUT JUST LIKE THE EXAMPLE ABOVE WITH NO SEPARATOR
==========
==========

You can use any character you want.
*Note! The *join()* method does not modify the existing arrays, instead it creates and returns a new one.
---------------------------------------------------------------------


# STRINGS TO ARRAYS
It is also possible to convert a *string* into an *array*, this can be done using the *split()* method.

The *split()* method takes a *separator* string as its argument.

This method splits the string at each point where the separator occurs.

<script>
    var string = "Making Serious Progress.";
    var arr = string.split(" ");
    document.write(typeof arr + ": " + arr);
</script>

HEAD OVER TO Strings-To-Array (Using-split-Method) TO SEE THE OUTPUT

*Note! The *split()* method does not modify the existing string, it creates a new array instead.

Here's another example:
<script>
    var string = "Making-Serious-Progress.";
    var arr = string.split("-");
    document.write(typeof arr + ": " + arr);
</script>

HEAD OVER TO Strings-To-Array (Using-split-Method2) TO SEE THE OUTPUT
---------------------------------------------------------------------

*Remember! The data type of *arrays* is *object*.

# MERGING ARRAYS
The *concat()* method merges two or more arrays.

<script>
    var animals = ["Lion", "Tiger", "Panther"];
    var animals2 = ["Dog", "Fowl", "Goat"];

    var arr = animals.concat(animals2);

    document.write(arr);
</script>

HEAD OVER TO Merging-Arrays (merge-array.html) TO SEE THE OUTPUT

To concatenate three or more arrays, separate the arrays with commas.

<script>
    var number1 = [1, 2, 3];
    var number2 = [4, 5, 6];
    var number3 = [7, 8, 9];

    var arr = number1.concat(number2, number3);
    document.write(arr);
</script>

HEAD OVER TO Merging-Arrays (concatenate-arrays.html) TO SEE THE OUTPUT  OF THIS CODE

*Note! The *concat()* method does not modify the existing arrays, instead it creates and returns a new one.
---------------------------------------------------------------------


# SEARCHING AN ITEM
The *indexOf()* method returns the index of the first occurence of an item (element) in the array.

<script>
    var animals = ["lion", "tiger", "dog", "cheetah"];

    var i = animals.indexOf("dog"); //returns 2
    document.write(i);
</script>

HEAD OVER TO Searching-An-Item (Using-indexOf.html) TO SEE THE OUTPUT OF THIS CODE
========
========

The *lastIndexOf()* method returns the index of the last occurenece of an item (element) in the array.

<script>
    var animals = ["lion", "tiger", "dog", "cheetah", "dog"];

    var i = animals.lastIndexOf("dog"); //returns 4
    document.write(i);
</script>

HEAD OVER TO Searching-An-Item (Using-lastIndexOf.html) TO SEE THE OUTPUT OF THIS CODE
========
========
* Remember! 0 is the index of the first element, 1 is the second element and so on.

Both *indexOf()* and *lastIndexOf()* methods return -1 if the item is not found in the array.

<script>
     var animals = ["lion", "tiger", "goat", "cheetah", "dog"];

    var firstIndex = animals.indexOf("zebra"); //returns -1
    var secondIndex = animals.indexOf("zebra"); //returns -1

    document.getElementById("demo").innerHTML =
    firstIndex + "<br>"
    secondIndex;
</script>

============
===========

To check if a value exists in an array, use the *includes()* method.

The *includes()* method returns *true* if a certain value is included in an array.

<script>
    var animals = ["Lion", "Tiger", "Dog"];

    var x = animals.includes("goat"); //returns false
    var y = animals.includes("lion"); //returns true

    document.getElementById("demo").innerHTML =
    x + "<br>"
    y;
</script>

HEAD OVER TO Searching-An-Item (Using-Includes-Method) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# SLICING AN ARRAY
The *slice()* method returns a new copy of a section of an array.

It takes two arguments.

1. *begin* - the index where the extraction begins
2. *end* - the index where the extraction should end (it is not included in the new aray).

<script>
    var animals = ["lion", "tiger", "dog", "goat"];
    var arr = animals.slice(0, 2)//returns ["lion", "tiger"]

    document.write(arr);
</script>

HEAD OVER TO Slicing-Array (Using-Slice-Method.html) TO SEE THE OUTPUT OF THIS CODE
========
========

Here's another example:

<script>
    var animals = ["lion", "tiger", "dog", "goat"];
    var arr = animals.slice(1, 3)//returns ["tiger", "goat"]

    document.write(arr);
</script>

*Note! The *slice()* method does not modify the existing arrays, instead it creates and returns a new one.
---------------------------------------------------------------------


# SPLICING AN ARRAY
The *splice()* method changes the contents of an array by removing or replacing existing elements and/or adding new elements in place.

It takes two or more arguments:

1. *start* - the index where the changing begins
2. *deleteCount* - the number of the elements to remove and replace from the *start*
3. *element1, element2, ...* - the elements to add to the array

<script>
    var months = ["January", "April", "May"];

    months.splice(1, 0, "Feburary", "March");
    document.write(months);
</script>

HEAD OVER TO Splicing-Arrays (Using-splice-method.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# REMOVING AN ARRAY ITEM
The *splice()* method can also be used to remove an array item.

To remove item/s, omit the third argument.

To remove a single item, specify the *index* of the item you want to remove and write 1, as the value of the *second argument*.

<script>
    var months = ["January", "April", "May"];

    months.splice(0, 1); //removes the first item
    document.write(months);
</script>

Here's another example:

<script>
    var months = ["January", "Feburary", "March", "April", "May"];

    months.splice(2, 1);
    document.write(months);
</script>

HEAD OVER TO Removing-Array (Using-splice-method.html) TO SEE THE OUTPUT
===========
===========

To remove multiple items, specify the index where you wan to start removing in the *first argument*, then specify the number of items you want to remove in the *second argument*.

<script>
    var months = ["January", "Feburary", "March", "April", "May"];

    months.splice(0, 2); //removes the first and second items
    document.write(months);
</script>

---------------------------------------------------------------------

# REPLACING AN ITEM'S VALUE
A much easier way to replace a single item's value is to access the item and assign a new value.

To access array's items, use their *index* number.

In the example below, we will replace *"Feburary"* with *"December"*.

<script>
    var months = ["January", "Feburary", "March", "April", "May"];

    months[1] = "December";

    document.write(months);
</script>

HEAD OVER TO Replacing-Array-Item (Replace-array.html) TO SEE THE OUTPUT