# JAVASCRIPT *for* LOOP
When programming, there are times that we need to run the *same statement* over and over again.

In this example, we accessed each value of the *fruits* array one by one.

<script>
    var fruits = ["apple", "mango", "orange"];
    var html = "";

    html += "<p>" + fruits[0] + "</p>";
    html += "<p>" + fruits[1] + "</p>";
    html += "<p>" + fruits[2] + "</p>";

    document.getElementById("demo").innerHTML = html;
</script>

The code above can be shortened using the *for* loop.

<script>
    var fruits = ["apple", "mango", "orange"];

    var html = "";

    for(var i = 0; i < fruits.length; i++){
        html += "<p>" + fruits[0] + "</p>";
    }

    document.getElementById("demo").innerHTML = html;
</script>

Notice that both examples above work the same way, but with different approaches.

HEAD OVER TO For-loop.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# WHAT IS A *for* LOOP?
A *for* loop executes statements repeatedly as long as the specified condition is met.

Syntax:

<script>
    for(initialExpression; condition; incrementExpression){
        // statements of code blocks
    }
</script>

* *initialExpression* - this initializes the loop counter.
* *condition* - if it is true, the loop statements executes, if false, the statements don't execute.
* *incrementExpression* - increments (increases) the loop counter, runs everytime the statements are executed.

The *statement* below will run 5 times. 

<script>
    for(var i = 0; i < 5; i++){
        document.write("<p>" Making progress "</p>");
    }
</script>

HEAD OVER TO For-Loop2.html TO SEE THE OUTPUT OF THIS CODE

In the example above, the loop is initialized with i = 0.

Next, the *condition* is defined, and *i* must be less than 5 for the loop to continue to run.

Then, the *i++* increments the counter everytime the code blocks are executed.

Once *i* is NO LONGER less than 5, the loop stops.

The *for* loop is commonly used with *arrays*.

<script>
    var cities = ["Seattle", "Oakland", "New York"];
    var html = "";

    for(var i = 0; i < cities.length; i++){
        html += "<p>" + cities[i] + "</p>";
    }

    document.getElementById("demo").innerHTML = html;
</script>