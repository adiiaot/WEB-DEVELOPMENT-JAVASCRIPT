# JAVASCRIPT STRINGS
In JavaScript, strings are pieces of text.

A *string* is a set of characters enclosed in quotes.

# CREATING STRINGS
Strings can be enclosed in double quotes (').

<script>
    var str = "Making Progress";
    document.write(str);
</script>

Strings can also be enclosed in single quotes (').

<script>
    var str = 'Making Progress';
    document.write(str);
</script>
---------------------------------------------------------------------


# SINGLE or DOUBLE QUOTES

Use *single* quotes if your string contains *double* quotes.

Use *double* quotes if your string contains *single* quotes.

<script>
    var str1 = "We'll win!";
    var str2 = "His name is 'Ayo Deji'";
    var str3 = 'His name is "Adii Aot"';

    document.getElementById("demo").innerHTML = 
    str1 + "<br>" +
    str2 + "<br>" +
    str3;
</script>

HEAD OVER TO Single-Double-Quotes (single-double.html) TO SEE THE OUTPUT

* If you use the quotes properly, your code would result into an error, because it will confuse the browser.

Let's test it out,

<script>
    var str = "Everything's fine;
    document.write(str);
</script>

DO THIS YOURSELF!, copy the code above into a new file and save it as Quotes.html, turn on the Live server or run it to see the output.
---------------------------------------------------------------------


# CONCATENATING STRINGS
To concatenate or add strings, use the addition operator (+).

<script>
    var str1 = "Making";
    var str2 = "Progress";

    var sentence = str1 + " " + str2;
    document.getElementById("demo").innerHTML = sentence;
</script>
RUN THIS CODE BY YOURSELF COPYING THIS CODE INTO A NEW FILE.

We can also concatenate strings using the addition assignment operator (+=)

<script>
    var str = "Making";

    str += "Progress";

    document.getElementById("demo").innerHTML = str; //prints out "Making Progress" as "Progress" gets assigned to the variable *str*
</script>

You can add as many strings as you want.

<script>
    var str1 = "I am Making";
    var str2 = "Serious";
    var str3 = "Progress";

    var sentence = str1 + " " + str2 + " " + str3;

    document.getElementById("demo").innerHTML = sentence;
</script>

HEAD OVER T0 Concatenating-Strings (concatenate.html) TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------



# CONCATENATION CONTEXTUAL EXAMPLE
In this example, we will create a program that greets the user by concatenating strings.

Also, we will use the window.prompt() to ask the user's name.

<script>
    function greetings(){
        var userName = window.prompt("Hello, welcome to the Javascript Tutorial, May I Know Your Name?");

        var str = "Nice to meet you " + user.Name + "Welcome to My Coding Course, I hope you are enjoying the lessons!";

        alert(str);
    }
</script>

HEAD OVER TO Sample-Files (Greetings.html) TO SEE THE OUTPUT OF THIS CODE

The entered value on the *prompt* was assigned to the *userName* variable. And then we applied concatenation to form a short greeting.

* Even the single space " ", that we put between the variables, is considered a *string*.   (can you imagine!)
---------------------------------------------------------------------

# ESCAPING CHARACTERS
Escaping characters is crucial in "handling strings".

It helps us make sure that our strings are recognized as pieces of text, not as part of the code.

To escape characters, use a backlash (\) right before the character.

<script>
    var str1 = "He is called \"Ayo Deji\""; //escaping "
    var str2 = 'He is called \'Adii Aot\''; //escaping '
    var str3 = "Escaping backlash \\"; //escaping \

    document.getElementById("demo").innerHTML = 
    str1 + "<br>" +
    str2 + "<br>" +
    str3;
</script>

HEAD OVER TO Escaping-Characters (escape.html) TO SEE THE OUTPUT IN YOUR BROWSER

* Escaping characters will avoid many common errors in writing strings.
---------------------------------------------------------------------


# BAD STRING
A bad string is a string that is not surrounded by quotes.

<script>
    var badString1 = I am a text;
    var badString2 = "I am a text;
    var badString3 = I am a text';
<script>

You should avoid these, because it will produce an error.