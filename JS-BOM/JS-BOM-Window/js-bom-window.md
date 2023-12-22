# WHAT IS THE BOM?
* *BOM* - stands for *Browser Object Model*

* *BOM* deals with browser components.

# THE WINDOW OBJECT
The window represents the current browser window.

All *variables* that were declared using the *var* keyword and *functions* declared in the global scope becomes properties of the *window* object.

<script>
    var txt = "Making Progress!";

    function sayHello(){
        // window.txt refers to the txt variable above
        document.write(txt);
    }
    // call sayHello() function using window object
    window.sayHello();
</script>

# WINDOW WIDTH AND HEIGHT
The *window* object contains the *innerWidth* and *innerHeight* properties.

These properties return the *width* and *height* of the current browser window in pixels.

HEAD OVER TO Window-size.html
---------------------------------------------------------------------


# WINDOW OBJECT PROPERTIES
The *window* object also contains the following objects:

* document
* screen
* location
* history
* navigator

In the next section, we will study the other window objects.