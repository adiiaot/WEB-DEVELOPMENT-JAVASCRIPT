# JAVASCRIPT ARRAY ITERATION
*Iterating over an array* means performing an operation for each array element.

Performed operations usually consist of accessing the value of each array element.

# USING *for* LOOP
The *for* loop can be used to iterate over an array.

Here's an example:

<script>
    var animals = ["Lion", "Tiger", "Dog"];

    for(var i = 0; i < animals.length; i++){
        document.write(animals[i] + "<br>");
    }
</script>

HEAD OVER TO Using-For-Loop.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# USING *forEach()* METHOD
The *forEach()* method executes a provided function once for each array element.

It has one parameter, a *callback function*.

The *callback function* accepts one to three arguments.

* *value*  - the current element being processed
* *index*  - the index of the current element
* *array*  - the array itself

The *index* and *array* variables can be omitted.

*Note! You can name the variables the way you like, as long as the names are not a *reserved keyword*.

Here's an example below:

<script>
    var animals = ["Tiger", "Dog", "Lion"];

    animals.forEach(function(value, index, array){
        document.getElementById("demo").innerHTML += "<p> Index: " + " <br>Value: " + value + "</p>";
    });
</script>

HEAD OVER TO Using-ForEach-method.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# USING *map()* METHOD
The *map()* function creates a new array.

Each element in the new array is changed using the logic in the provided function.

The *provided function* accepts one to three arguments.

* *value* - the current element being processed
* *index* - the index of the current element
* *array* - the array itself

The *index* and *array* arguments can be omitted.

In the example below, each element in the *numbers* array is multiplied by *2*.

<script>
    var numbers = [10, 20, 30, 40, 50];

    var numbersTimesTwo = numbers.map(function(value, index, array){
        return value * 2;
    });

    document.getElementById("demo").innerHTML += numbersTimesTwo;
</script>

HEAD OVER TO Using-Map-Method.html TO SEE THE OUTPUT OF THIS CODE

*NOTE! The *map()* function does not modify the existing array*
---------------------------------------------------------------------


# USING *filter()* METHOD
The *filter()* method creates a new array.

The new array only contains the elements that passed the test implemented by the provided *provided function*.

The *provided function* accepts one to three arguments.

* *value* - the current element being processed
* *index* - the index of the current element
* *array* - the array itself

The *index* and *array* arguments can be omitted.

In the example below, only the numbers less than *4* are passed to the new array.

<script>
    var numbers = [1, 2, 3, 4, 5];

    var newArr = numbers.filter(function(value){
        return value < 4;
    });

    document.getElementById("demo").innerHTML += newArr;
</script>

HEAD OVER TO Using-Filter-method.html TO SEE THE OUTPUT OF THIS CODE
 
*NOTE! The *filter()* function does not modify the existing array.