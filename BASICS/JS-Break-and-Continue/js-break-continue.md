# JAVASCRIPT *Break* AND *Continue* 
The *break* and *continue* statements are often used in *loops*.

# THE *break* STATEMENT
You have already learnt that the *break* statement is used to stop the execution of the *switch* statement.

In this section, we will learn how to use the in loops.

The *break* statement terminates the execution of the current loop.

After termination, the execution proceeds to the next statement following the loop.

<script>
    var html = "";
    for(var i = 0; i < 10; i++){
        if(i == 5){
            break;
        }
        html += "<li>Number " + i + "</li>"; //add string to html
    }

    document.getElementById("demo").innerHTML = html;
</script>

HEAD OVER TO Break.html TO SEE THE OUTPUT OF THIS CODE

As you may notice, instead of printing 10 numbers, only 5 numbers were printed.

It is because when *i* became equal to *5* the next iteration was stopped using the *break* statement.

After that, the program executed the following statement that printed the *html* string, instead of adding more strings to the *html* variable.
---------------------------------------------------------------------


# THE *continue* STATEMENT
The *continue* statement terminates execution of the statements in the current iteration of the current loop.

And continues the execution of the loop with the *next iteration*.

<script>
    var html = "";
    for(var i = 0; i < 10; i++){
        if(i == 5){
            continue;
        }
        html += "<li>Number " + i + "</li>"; //add string to html
    }

    document.getElementById("demo").innerHTML = html;
</script>

HEAD OVER TO Continue.html TO SEE THE OUTPUT OF THIS CODE

As you may notice, in the other example, only "Number 5" was missing.

It is because the *continue* statement terminated the execution of the current iteration when *i* became equal to 5.

After that, the program continued the executio of the *next iteration*.