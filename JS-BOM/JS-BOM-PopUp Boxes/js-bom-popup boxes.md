# JAVASCRIPT BOM POP-UP BOXES
With JavaScript, we can show pop-up (dialog) boxes to the user.

There are three types of pop-up boxes:

* Alert Pop-up Box
* Confirm Pop-up Box
* Prompt Pop-up Box

# ALERT POP-UP BOX
The *window.alert()* method lets us display a pop-up box with a specified content and an "OK" button.

You can use *window.alert()* without the *window* prefix.

<script>
    alert("Making Progress");
</script>


# CONFIRM POP-UP BOX
The *window.confirm()* method displays a pop-up box with a message and two button: "OK" and "Cancel"

It returns a Boolean indicatin g whether "OK" (true) or "Cancel" (false) was selected.

<script>
    if(confirm("Are you making progress?")){
        alert("You pressed OK. Well done");
    }else {
        alert("You pressed cancel.");
    }
</script>

HEAD OVER TO Confirm.html
---------------------------------------------------------------------


# PROMPT POP-UP BOX
The *window.prompt()* method displays a pop-up box with a message asking the user for a text input.

It returns a *string* containing the text entered by the user.

If the user did not enter a value, it returns an empty string or null.

HEAD OVER TO Prompt.html