# JAVASCRIPT *while* LOOP
The *while* loop executes statements as long as the given condition evalutates to *true*.

Syntax: 
<script>
    while(condition){
         // statements or code blocks
    }
</script>

* *condition* - the expression evaluated, if it evaluates to true, the code blocks are executed, if false, the loop stops.

* *statements* - the code blocks to be executed as long as the condition is true

Here's a basic example:

<script>
    var i = 0;

    while(i < 3){
        document.write("<p> Making progress </p>");
        i++;
    }
</script>

In the example above, the *statement* is executed 3 times.

It is because the *statement* only stopped running when *i* is NO LONGER less than 3.
---------------------------------------------------------------------


# LOOPING OVER AN ARRAY USING *while* LOOP
To loop over an array, declare a variable that holds the *length* of the *array*.

Then use it in the *condition*.

<script>
    var animals = ["Lion", "Tiger", "Dog"];
    var len = fruits.length;
    var i = 0;
    var html = "";

    while(i < len){
        html += "<p> I like " + fruits[i] + ". </p>";
        i++;
    }

    document.getElementById("demo").innerHTML = html;
</script>

HEAD OVER Looping-Array.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *do....while* LOOP
The *do...while* loop executes statements until the test condition evaluates to *false*.

Syntax: 

<script>
    do{
        // statements or code blocks
    } while (condition);
</script>

* *statements* - the code blocks executed and is reexecuted each time the *condition* is true.

* *condition* - the expression evaluated, if it evaluates to true, the code blocks re-execute if false, the loop stops.

Here's a basic example:

<script>
    var i = 0;
    do{
        document.write("<p> Making progress </p>");
        i++;
    }while(i < 3);
</script>

In the example above, the *statement* is executed 3 times.

It is because the *statement* only stopped running when *i* is NO LONGER less than 3.
---------------------------------------------------------------------


# LOOPING OVER AN ARRAY USING *do...while* LOOP
We can also use the *do...while* loop over an array.

<script>
     var animals = ["Lion", "Tiger", "Dog"];
     var len = animals.length;
     var i = 0;
     var html = "";
    
        do{
            html += "<p> Someday, I will buy a " + animals[i] + ". </p>";
            i++;
        }while(i < len);

        document.getElementById("demo").innerHTML = html
</script>

HEAD OVER TO looping-Arrays-Do.html  TO SEE THE OUTPUT OF THIS CODE