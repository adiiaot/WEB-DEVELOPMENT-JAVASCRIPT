# JAVASCRIPT *switch* STATEMENT
In programming, there are times that we need multiple *if* statements.

In the example below, the program prints the color of the given fruit by checking what fruit is specified.

<script>
    var fruit = "mango";

    if(fruit == "apple"){
        document.write("The color is red.");
    }
    if(fruit == "strawberry"){
        document.write("The color is pink.");
    }
    if(fruit == "mango"){
        document.write("The color is yellow");
    }
</script>

As you may notice, the code above looks inefficient.

Instead of writing multiple *if* statements, we can shorten the code above with the *switch* statement.

<script>
    var fruit = "mango";

    switch(fruit){
        case "apple":
            document.write("The color is red");
            break;
        case "strawberry":
            document.write("The color is pink");
            break;
        case "mango":
            document.write("The color is yellow");
            break;
    }
</script>

HEAD OVER TO Fruit.html TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *switch* STATEMENT
The *switch* statement matches an expression against the specified values in the *case* clauses.

Syntax:

<script>
    switch(expression) {
        case value1:
            // code blocks to be executed
            break;
        case value2:
            // code blocks to be executed
            break;
        case value3: 
            // code blocks to be executed
            break;
    }
</script>

The *switch* statement evaluates the expression to *value1* first, then to *value2* and so on.

If the expression matches a value, the associated *code blocks* are executed.

Here's a basic example:
<script>
    var city = "Abuja";

    switch(city){
        case "Abuja":
            document.write("The Federal Capital of Nigeria");
            break;
        case "Washington, DC":
            document.write("The Capital city of USA");
            break;
        case "Mumbai":
            document.write("The Capital city of India");
            break;
    }
</script>

*Note! The evaluations are sensitively cased.* 
---------------------------------------------------------------------


# THE *break* KEYWORD
The *break* keyword comes after the *code blocks* of each *case* clause.

Although it is optional, it is highly recommnended.

The role of the *break* keyword is to *stop the execution* of the *switch* statement when an evaluation already matches a case.