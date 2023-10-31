# JAVASCRIPT ARRAY SORTING
In this section, we will learn how to sort arrays using *Array* methods.

# THE *sort()* METHOD
The *sort()* method sorts the elements of an array.

*Ascending* is the default sort order.

In the example below, the array is sorted alphabetically.

<script>
    var animals = ["Bear", "Ant", "Dog", "Lion"];
    animals.sort();

    document.write(animals);
</script>

HEAD OVER TO The-Sort-Method (using-sort-method.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE COMPARE FUNCTION
The *sort()* method can take one argument, a compare function.

The *compare function* defines the sort order. It is is omitted (like the example above), array elements are converted to string then sorted according to each character's *Unicode* code point value.

The *compareFunction()* comes with two arguments *a* and *b*.

If *a* and *b* are two elements being compared, then:

* if *compareFunction(a, b)* returns less than 0, *a* comes first.

* if *compareFunction(a, b)* returns 0, *a* and *b* are unchanged.

* if *compareFunction(a, b)* returns greater than 0, *b* comes first.

The examples below use *compare functions*.
---------------------------------------------------------------------


# SORTING NUMBERS
To sort numbers in an array, we should use a compare function.

In the example below, the numbers are sorted in *ascending order*.

<script>
    var numbers = [5, 3, 4, 1, 2];
    numbers.sort(function(a, b){
        return a - b;
    });

    document.write(numbers);
</script>

You can also separate your compare function

<script>
    var numbers = [5, 3, 4, 1, 2];
    numbers.sort(compareFunction);

    function compareFunction(a, b){
        return a - b;
    }
    document.write(numbers); //prints out 1,2,3,4,5
</script>

HEAD OVER TO Sorting-Numbers (Using-CompareFunction.html) TO SEE THE OUTPUT OF THIS CODE
======
=====

In the example below, the numbers are sorted in *descending order*.

<script>
    var numbers = [5, 3, 4, 1, 2];
    numbers.sort(compareFunction);

    function compareFunction(a, b){
        return b - a;
    }
    document.write(numbers); //prints out 5,4,3,2,1
</script>
---------------------------------------------------------------------

# GET THE HIGHEST OR LOWEST VALUE
To get the *highest* value in an array of numbers, sort the elements in *descending order* then get the first value.

<script>
    var numbers = ["3", "5", "2", "1", "4"];
    numbers.sort(compareFunction);

    function compareFunction(a, b){
        return  b - a;
    }

    var highest = number[0]; //gets the first value of the order

    document.write(highest);
</script>

HEAD OVER TO Getting-Highest-Lowest-Value (Highest-Value.html) TO SEE THE OUTPUT OF THIS CODE

* To get the *lowest* value in an array of numbers, sort the element is *ascending order* then get the first value.

<script>
    var numbers = ["3", "5", "2", "1", "4"];
    numbers.sort(compareFunction);

    function compareFunction(a, b){
        return a - b;
    }

    var lowest = numbers[0];

    document.write(lowest);
</script>

HEAD OVER TO Getting-Highest-Lowest-Value (Lowest-Value.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# SORTING AN ARRAY OF OBJECTS
To sort an array of objects, simply compare the object's numerical properties.

<script>
    var students = [
        {name: "Ayo", age: 8},
        {name: "Adii", age: 5},
        {name: "Taye", age: 3}
    ];

    students.sort(function(a, b){
        return a.age - b.age;
    });

    /* displaying the data */
    for(var i = 0; i < students.length; i++){
        document.getElementById("demo").innerHTML += "<p>Name: " 
        + students[i].name + "<br> Age: " + students[i].age + "</p>";
    }
</script>

HEAD OVER TO Sorting-Array-of-Objects (Array-of-Objects.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# REVERSING AN ARRAY

The *reverse()* method reverses an array.

<script>
    var animals = ["lion", "dog", "ant", "bear"];

    animals.reverse();

    document.write(animals);
</script>

HEAD OVER TO Reversing-Array (reversing-array.html) TO SEE THE OUTPUT OF THIS CODE.