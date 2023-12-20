# JAVASCRIPT DOM EFFECTS
With CSS, JAVASCRIPT and DOM we can create effects that can be applied to elements.

# FADING EFFECTS
In this section, we will show or hide elements with a fading effect.

First, we need to create and style an element.

Let's create a <div> element with the following styles.

<html>
<head>
    <title></title>
    <style type = text/css >
        div#demo {
            width: 200px;
            height: 200px;
            background: green;

            opacity: 1s; /* default */
            display: block; /* default */


            /* this will animate the element for 1 second when its properties change */
            transition: all 1s;
        }
    </style>
</head>
    <body>
    </body>
</html>

The *transition: all 1s* CSS declaration will animate the element for 1 second whenever we make changes to its properties.
=====================================================================


# FADE OUT
To *fade out* an element, set its *opacity* property to 0 using JavaScript.

To completely hide it, set the *display* property to *none*.

But we have to wait 1 second (time specified in *transition* property), before completely hiding the element so that we can see the fading effect.

HEAD OVER TO FadeOut.html
---------------------------------------------------------------------


# FADE IN
To *fade in* an element, set its *display* and *opacity* properties to *block* and 1 respectively.

HEAD OVER TO FadeIn.html
---------------------------------------------------------------------


# SLIDING EFFECT
To make a sliding effect, use the *max-height* and *overflow-y* CSS properties.

Set the *max-height* property to the approximae height of the element.

And set the *overflow-y* property to *hidden*.

<style type= text/css >
    ul#demo {
        max-height: 100px;
        overflow-y: hidden;

        /* this will animate the element for 1 second when its properties change */
        transition: all 1s;
    }
</style>

To *slide-up* the element, set the max-height CSS property to 0 using JavaScript.

To slide-down, set the max-height property to its approximate height (in this case, we use 100px).

HEAD OVER TO Sliding-effect.html