# JAVASCRIPT ARROW FUNCTION
The *arrow function* expression is a compact alternative to a regular function expression.

For example:

<script>
    function myFunc(){
        alert("Making Progress");
    }
</script>

The example above is similar with this:

<script>
    const myFunc() = () => {
        alert("Making Progress");
    }
</script>

If you only have one statement, you can omit the curly brackets {}.

<script>
    const myFunc() = () => alert("Making Progress");
</script>

---------------------------------------------------------------------


# PARAMETERS IN ARROW FUNCTION
Parameters in an arrow function should be inside the parantheses ().

<script>
    const myFunc() = (x, y) => alert(x + y);
</script>

If you have only one parameter, you can omit the parantheses ().

<script>
    const myFunc() = animal => alert("I want to buy a " + animal);
</script>

HEAD OVER TO Arrow.html
---------------------------------------------------------------------


# *this* IN ARROW FUNCTION
In a regular function, the *this* keyword represents the *global object* or the object that called it.  e.g HTML button element.

On the other hand, the *this* keyword in an arrow function always represents the *object that owns it*.

No matter what calls it.

The example below aims to change the styles of the button when it's clicked.

However, the button's styles will NOT be changed because the *changeStyle()* function is owned by the *window* object.

Therefore, the *this* keyword represents the *window* object, not the HTML button element.

<script>
    const btn = document.getElementById("btn");

    const changeStyle = () => {
        this.style.background = "red";
        this.style.color = "white";
    };

    btn.onclick = function(){
        changeStyle();
    };
</script>

To change the styles of the button, the *changeStyle()* function must be owned by the HTML button element.

This way, the *this* keyword will represent the HTML button element.

<script>
        const btn = document.getElementById("btn");

        btn.onclick = function(){
          const changeStyle = () => {
             this.style.background = "red";
             this.style.color = "white";
         };
              changeStyle();
        };
</script>

HEAD OVER TO This-arrow.html