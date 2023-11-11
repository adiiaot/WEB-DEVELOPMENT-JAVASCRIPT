# JAVASCRIPT REGULAR EXPRESSIONS
*Regular Expressions* are patterns used to match character combinations to strings.

In this section, we will study the basics of Regular Expressions

Regular Expressions are commonly used to *search* or *replace* a piece of text from a string.

# CREATING A REGULAR EXPRESSION
To create a regular expression, follow this syntax:

<script>
    var pattern = /pattern/modifiers;
</script>

EXAMPLE:

<script>
    var pattern = /adiidevs/gi;
</script>

The *pattern* is enclosed by *slashes*.

The *modifiers* are optional.

Another way of creating a regular expression is by using the *RegExp* class.

<script>
    var pattern = new RegExp('pattern', 'modifiers');
</script>

EXAMPLE:


<script>
    var pattern = new RegExp('adiidevs', 'gi');
</script>

Simply enclose the *pattern* and *modifiers* by quotation marks.
---------------------------------------------------------------------


# WHEN DO WE USE REGULAR EXPRESSIONS
In JavaScript, regular expressions are commonly used when searching and replacing text from a string.

Thus, they are commonly used with the *search()* and *replace()* and other similar methods.

Both these methods are explained in this section.
---------------------------------------------------------------------


# USING REGULAR EXPRESSIONS WITH *search()*
The *search()* method returns the *index* of the FIRST OCCURENCE of a text in a string. It is case-sensitive.

It returns -1 if no match is found.

<script>
    var text = "Making Progress";
    var search = text.search("Making");
    document.write(search);
</script>

HEAD OVER TO Using-Search-Method (search.html) TO SEE THE OUTPUT OF THIS CODE

Here's an example of using it with a regular expression

<script>
    var text = "Making Progress";
    var search = text.search(/pRoGrEsS/i);
    document.write(search);
</script>

HEAD OVER TO Using-Search-Method (regular-expression.html) TO SEE THE OUTPUT OF THIS CODE

In the example above, we used the *i* modifier which makes the search case-sensitive
---------------------------------------------------------------------


# USING REGULAR EXPRESSIONS WITH *replace()* 
The *replace()* method replaces the specified text inside a string and returns a new string, It is case-sensitive.

<script>
    var text = "JavaScript is fun, I am like JavaScript";
    var replace = text.replace("JavaScript", "Gaming");
    document.write(replace);
</script>

HEAD OVER TO Using-Replace-Method (replace.html) TO SEE THE OUTPUT OF THIS CODE

Notice that only the first occurence of "Javascript" was replaced.

To replace all occurences, use a regular expressiom with the *g* modiifer.

<script>
    var text = "JavaScript is fun, I am like JavaScript";
    var replace = text.replace(JavaScript/g, "Gaming");
    document.write(replace);
</script>

HEAD OVER TO Regular-expression.html TO SEE THE OUTPUT OF THIS CODE

We can also combine the *g* and *i* modifier in a single regular expression.

<script>
    var text = "JavaScript is fun, I am like JavaScript";
    var replace = text.replace(JaVaScRiPt/gi, "Gaming");
    document.write(replace);
</script>

HEAD OVER TO Regular-combine.html TO SEE THE OUTPUT OF THIS CODE