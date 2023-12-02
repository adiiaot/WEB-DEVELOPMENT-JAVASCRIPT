# JAVASCRIPT FORMS
*HTML FORMS* can be validated using JavaScript before they are submitted to a server.

*Note! YOU MUST HAVE KNOWLEDGE OF HTML FORMS BEFORE TAKING THIS SECTION*

# HOW TO PREVENT A FORM BEING SUBMITTED
An HTML form can be prevented from being submitted by using *return false* when the form received the *submit* event.

<html>
    <form action = "https://adiidevs.com/form-action.php" onsubmit = "return validateForm()">
        <input type = "text" name = "firstName" />
        <input type = "submit" />
    </form>
</html>

The *form* above will not be submitted when we use *return false* in the event handler.

Notice that we also used *return* in the *onsubmit* attribute.

<script>
    function validateForm(){
        alert("This form will not be submitted");
        return false;
    }
</script>


# CLIENT-SIDE VALIDATION
Client-side form validation is done by a web page before sending input data to a server.

In this example, if the *text field* is EMPTY, the input data will not be submitted to the server.

<script>
    function validateForm(){
        const firstName = document.getElementById("firstName").value;
        if(firstName == ""){
            alert("Please enter a value on the text field");
            return false;
        }
    }
</script>

HEAD OVER TO client.html

The *https://adiidevs.com/form-action.php* is a server-side script