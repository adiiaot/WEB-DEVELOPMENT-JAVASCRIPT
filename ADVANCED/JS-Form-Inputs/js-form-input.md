# JAVASCRIPT FORM INPUTS
In this section, we will study how to validate form inputs.

# HOW TO GET AN INPUT'S VALUE
Before we can learn ho to validate inputs, we need to know how to get their value first.

To get an input's value, select the element and use its *value* property.


<script>
    function getValue(){
        const val = document.getElementById("firstName").value;
        alert("The value is " + val);
    }
</script>

HEAD OVER TO Get-value.html

Notice that in the example above, we used the *document.getElementById()* method to select the input element.

A more efficient way to select an input element is the *document.getElementByName()* method

This way, we don't have to put *Id's* in each input.
    <script>
        function getValue(){
            const val = document.getElementsByName("firstName")[0].value;
            alert("The value is " + val);
        }
    </script>

HEAD OVER TO Get-input.html

The *document.getElementsByName()* returns an array of selected elements with the speciifed *name*.

That's why we used bracket notation () [0] to select the first item
---------------------------------------------------------------------


# VALIDATE EMPTY TEXT INPUT

The form below will not be submitted if the *firstName* input is empty

<script>
    function validateForm(){
        const firstName = document.getElementsByName("firstName");
        if(firstName == ""){
            alert("This form will not be submitted");
            return false;
        }
    }
</script>

HEAD OVER TO Empty-input.html
---------------------------------------------------------------------


# LIMIT NUMBER OF CHARACTERS
The form below will not be submitted if the user inputs a text exceeding 10 character

<script>
    function validateForm(){
        const userName = document.getElementsByName("userName")[0].value;
        const length = userName.length;
        if(length > 10){
            alert("You cannot input more than 10 characters");
            return false;
        }
    }
</script>

HEAD OVER TO Limit-character.html
---------------------------------------------------------------------


# VALIDATE NUMBERS
The form below will not be submitted if the user inputs a number below 18.

<script>
    function validateForm(){
        const age = document.getElementsByName("age")[0].value;
        if (age < 18){
            alert("The age of the user is less than 18");
            return false;
        }
    }
</script>

=====================================================================


# USING HTML5 ATTRIBUTES
HTML5 introduced new attributes that can help validate forms.

For example, the *required* attribute will prevent a form from being submitted if the input is empty.

<!DOCTYPE html>
<html>
<head>
<title>USING THE *required* ATTRIBUTE</title>
</head>
<body>
    <form>
        <label>First Name: <input type= "text" name = "firstName" required /></label>
        <input type= "submit" />
    </form>
</body>
</html>

The *min* and *max* attributes specify the minimum and maximum input values allowed.

In this example, only numbers form 18-65 are allowed.

<html>
<head>
<title>USING THE *required* ATTRIBUTE</title>
</head>
<body>
    <form>
        <label>Age: <input type="number" name="age" min="18" max= "65" required /></label>
        <input type= "submit" />
    </form>
</body>
</html>

HEAD OVER TO required.html