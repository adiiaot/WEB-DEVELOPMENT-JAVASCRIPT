# JAVASCRIPT STRING METHODS
Now that we already know the basics of strings, let's move up and try some useful operations that we can do with it.

# STRINGS AS OBJECTS

Almost everything in JavaScript is objects.

When you create a string:

<script>
    var str = "Making Progress";
</script>

Your variable becomes a *string* object instance.

As a result, many properties and methods are available to it.
---------------------------------------------------------------------

# GETTING STRING LENGTH
To get the length or the number of characters in a string, use the *length* property.

<script>
    var str = "Adiidevs";
    var strlen = str.length;

    document.write(strlen); //prints out 8 
</script>

HEAD OVER TO String-Length (string-Length.html) TO SEE THE NUMBER OF CHARACTERS IN YOUR BROWSER

The *length* property is useful, for instance, you can use it to count how many characters a user has entered in one of your text fields.

It can help you write a program that will tell the user to shorten their entity.
---------------------------------------------------------------------


# RETRIEVING A CHARACTER
We can retrieve a character from a string using the *square bracket notation*.

Simply put *square brackets []* after the variable name and write a number inside them.

<script>
    var str = "Adiidevs";
    var x = str[6];

    document.write(x); //prints out v
</script>

HEAD OVER TO Retrieving-Characters (retrieve.html) TO SEE THE OUTPUT OF THIS CODE

You may have expected that *str[6]* would return the 5th character "e" from the "Adiidevs" string.

But instead it returned the 6th character which is "v".

It is because JavaScript counts from 0, not from 1.

Thus, 0 represents the first character, 1 represents the second character and so on.

* Note: The number inside the square brackets [] is called *index*.
---------------------------------------------------------------------


# FINDING A SUBSTRING IN A STRING
Sometimes, it is useful to check if a smaller string (substring) is present in a string.

This can be done using the *indexOf()* method.

It returns the *index* of the FIRST occurence of a substring in a string.

<script>
    var str = "Where are they, where did they go.";
    var strpos = str.indexOf("they");

    document.write(strpos);
</script>

-----------
-----------

* The *lastIndexOf()* method returns the *index* of the LAST occurence of a substring in a string.

<script>
    var str = "Where are they, where did they go.";
    var strpos = str.lastIndexOf("they");

    document.write(strpos);
</script>

--------
--------

Both the *indexOf() and the *lastIndexOf()* methods return -1 if there is no occurence found.

<script>
    var str = "Where are they, where did they go.";
    var strpos1 = str.indexOf("Adiidevs"); //returns -1
    var strpos2 = str.lastIndexOf("Adiidevs"); //returns -1

    document.getElementById("demo").innerHTML = strpos1 + "<br>" +
    strpos2;
</script>
---------------------------------------------------------------------


# THE SEARCH() METHOD
The *search()* method works similarily with the *indexOf()* method.

It returns the *index* of the FIRST occurence of a text in a string.

<script>
    var str = "Where are they, where did they go.";
    var strpos = str.search("they");

    document.write(strpos);
</script>

HEAD OVER TO Search-Method (search.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------

The *search* method is sensitively cased. To search a text insensitively, use a simple regular expression with the */i* flag.

<script>
    var str = "Making Progress!";
    var strpos = str.search(/making/i); //returns M

    document.write(strpos);
</script>
---------------
--------------

Don't forget. The counting starts from 0. Therefore, 0 represents the FIRST CHARACTER.

The *search()* method returns -1 if the text is not found in the string.

<script>
    var str = "Where are they, where did they go.";
    var strpos = str.search("Adiidevs"); //returns -1 as Adiidevs is not present in the str variable string

    document.write(strpos);
</script>
---------------------------------------------------------------------


# EXTRACTING A STRING
We can extract a substring from a string using the following methods:

* slice(start, end)
* substring(start, end)
* substr(start, length)

# THE *slice()* METHOD
The *slice()* method extracts a section of a string and returns it as a new string.

It does not modify the original string.

It takes two numerical parameters: the start *index* (position), the end *index*

<script>
    var str = "The quick brown fox jumps over the lazy dog.";
    var result = str.slice(10, 19);

    document.write(result);
</script>

HEAD OVER TO Slice-Method (slice.html) TO SEE THE OUTPUT OF THIS CODE

The *slice()* method can take negative values.

Negative values start counting from the end of the string.

<script>
    var str = "The quick brown fox jumps over the lazy dog.";
    var result = str.slice(-9, -1);

    document.write(result);
</script>

HEAD OVER TO Slice-Method (slice2.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# THE *substring()* METHOD
The *substring()* method works the same way as the *slice()* method.

<script>
    var str = "The quick brown fox jumps over the lazy dog.";
    var result = str.substring(10, 19);

    document.write(result);
</script>
HEAD OVER TO Substring-Method (substring.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------

The only difference between *slice()* and *substring()* methods is that the *substring()* method cannot take negative values.


# THE *substr()* METHOD
The *substr()* method extracts a section of a string, starting from a specified *index* and extending for a given *length* afterwards.

It takes two numerical parameters: the starting *index*, the *length* - number of characters to extract

<script>
    var str = "The quick brown fox jumps over the lazy dog.";
    var result = str.substr(10, 9);

    document.write(result);
</script>

HEAD OVER TO Substr-Method (substr.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------



# OMITTING THE SECOND VALUE
If you omit the second value of *slice()*, *substring()* and *substr()*, they will return the rest of the string.

<script>
    var str = "The quick brown fox jumps over the lazy dog.";
    var result1 = str.slice(10);
    var result2 = str.substring(10);
    var result3 = str.substr(10);

    document.getElementById("demo").innerHTML = 
    result1 + "<br>" +
    result2 + "<br>" +
    result3;

</script>
---------------------------------------------------------------------


# REPLACING STRING INSIDE A STRING
The *replace()* method replaces the specified text inside a string and returns a new string.

It does not modify the original string.

It takes two parameters: the *string to replace*, the string replacement.

<script>
    var str = "Adiidevs is nice, I love Adiidevs!";
    var result = str.replace("Adiidevs", "Adiiaot");

    document.write(result);
</script>

HEAD OVER TO Replace-Method (replace.html) TO SEE THE OUTPUT OF THIS CODE

Notice that only the first occurence of "Adiidevs" was changed.

To replace all matching strings, use a regular expression with the */g* flag.

<script>
    var str = "Adiidevs is nice, I love Adiidevs!";
    var result = str.replace(/Adiidevs/g, "Adiiaot");

    document.write(result);
</script>
HEAD OVER TO Replace-Method (replace2.html) TO SEE THE OUTPUT OF THIS CODE

Now all occurences of "Adiidevs" are replaced by "Adiiaot".

Note! The *replace()* method is sensitively cased.

To replace text insensitively, use the /i flag in the regular expression.

<script>
    var str = "Adiidevs is nice, I love Adiidevs!";
    var result = str.replace(/AdiiDevs/i, "Adiiaot");

    document.write(result);
</script>

HEAD OVER TO Replace-Method (replace3.html) TO SEE THE OUTPUT OF THIS CODE

As you may notice again, it only replaced the first occurence.

To replace all insensitively, combine the /g and /i flags in the regular expression

<script>
    var str = "Adiidevs is nice, I love Adiidevs!";
    var result = str.replace(/AdiiDevs/gi, "Adiiaot");

    document.write(result);
</script>

HEAD OVER TO Replace-Method (replace4.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# TRIMMMING A STRING
Trimming means removing the extra whitespaces from both ends of a string.

<script>
    var str = "    I love AdiiDevs!     ";
    var result = str.trim();

    alert(result);
</script>
HEAD OVER TO Trimming-String (Trim.html) TO SEE THE OUTPUT OF THIS CODE
-----------------------------------------------------------------


# CONVERTING TO UPPER AND LOWER CASE

The *toUpperCase()* method converts the string to upper caser.

It only returns the converted value and does not modify the original string.

<script>
    var str = "I love AdiiDevs!";
    var result = str.toUpperCase();

    document.write(result);
</script>

HEAD OVER TO Converting-To-Upper-Lower-Case (to-uppercase.html) TO SEE THE OUTPUT OF THIS CODE

The *toLowerCase()* method converts the string to the lower case.

It only returns the converted value and does not modif the original string.

<script>
    var str = "I LOVE AdiiDevs!";
    var result = str.toLowerCase();

    document.write(result);
</script>

HEAD OVER TO Converting-To-Upper-Lower-Case (to-lowercase.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------



# THE *concat()* METHOD
The *concat()* method adds the string arguement to the function calling string without modifying the original string.

It takes two arguements: the text that would separate the strings, the string to add.

<script>
    var str = "Lorem";
    var result = str.concat(" ", "ipsum");

    document.write(result); 
</script>

In the example above, the strings are separated by a whitespace " ".

You can also use other characters like a comma (,).
<script>
    var str = "Lorem";
    var result = str.concat("," "ipsum");

    document.write(result); 
</script>

Try it out in a new file.