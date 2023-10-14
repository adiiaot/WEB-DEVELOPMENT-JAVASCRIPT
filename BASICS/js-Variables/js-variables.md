# JAVASCRIPT VARIABLES

In programming or algebra, we use the variables to hold values.

In JavaScript, variables are used to *store data*

The data stored could be a "text", a "number" or others.

Making use of variables in JavaScript is very easy. Here is how:

<script>
    var firstName = "Adii";
    var lastName = "Aot";
    var age = 17;

    //printing the values
    document.write(firstName + "" + lastName + "<br>");
    document.write(age);
</script>

HEAD OVER TO THE variables.html FILE to see the output of the code above.


As you can see,
* The text "Adii" is stored/assigned to firstName
* The text "Aot" is stored/assigned to lastName
* The number 17 is stored/assigned to age


*NOTE: You should give meaningful names to your variables as much as possible, this helps maintain the readability of your code.
---------------------------------------------------------------------


# DECLARING A VARIABLE

The "var" statement creates or declares a variable.

In the example below, the variable x is declared and is initialized/assigned to the value 17.

<script>
    var x; //declares the variable as x
    x = 17; //assigns/initializes x to 17

    document.write(x); //prints out the value of x which is 17
</script>

HEAD OVER TO declaringvariables.html FILE to see the output of this code


# DECLARING MULTIPLE VARIABLES IN ONE STATEMENT
It is possible to declare multiple variables at once, using a single statement.

Simply separate the variables with a comma (,).

<script>
    var firstName = "Adii", lastName = "Aot", age = 17; //declares the variables firstName, lastName and age

    //printing the values
    document.write(firstName + " " lastName + "<br>");
    document.write(age);
</script>

HEAD OVER TO multipleVariables.html to see the output of this code

*NOTE: If you have multiple variable-named words, it is recommended to use the *camelCase* way, just like what we did with the "firstName" and "lastName".
---------------------------------------------------------------------


# THE EQUAL SIGN

As you may notice, we have been using the equal sign to assign values or data to variables.

The equal sign (=) is called the *assignment operator*

* THE DATA STORED/ASSIGNED
The data stored could be a text, number etc. These are called *data types*

You will learn about them in the next folder(Navigate to the "Where-to-start.md" to stay upto date with the folders to open next)


# NAMING VARIABLES
JavaScript variables should be identified with unique names.

These unique names are called *identifiers*

* Identifiers can be short as a single letter like x, y, z, i, a, b ... any alphabet or word such as firstName, lastName, twinTower, adiiDevs...etc

# RULES FOR NAMING VARIABLES
Yeah, there are rules for naming variables. You can't just name it like a password, yeah am telling you JavaScript is a script.
 
Here are the rules:

1. A variable name should start with a letter (a,b,c...), an underscore (_), or a dollar sign($)

2. A name cannot start with a number (1,2,3...)

3. A name can only contain letters, digits, underscores and dollar signs.

4. JavaScript reserved keywords like (var, function, if, let, else, foreach, for, in, this, while, const...etc) cannot be used as variable names.