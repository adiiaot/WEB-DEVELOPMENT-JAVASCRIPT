# JAVASCRIPT CLASSES
JavaScript classes are a special type of functions.

# DECLARING A CLASS
To declare or create a class, use the *class* keyword with the name of the class.

In this example, the *fruit* class is created.

<script>
    class Fruit {
        constructor(fruitName) {
            this.name = fruitName;
        }
    }
</script>

*NOTE! Class declarations are not hoisted.*

Now we can use and/or initialize the *fruit* class using the *new* operator.

<script>
    const fruit = new Fruit("apple");
</script>

After calling *new Fruit("apple")*, an object is created.

Then, the *constructor()* runs automatically with the given argument and assigns *this.name* to the created object.

<script>
    class Fruit {
        constructor(fruitName){
            this.name = fruitName;
        }
    }

    const fruit = new Fruit("apple");

    //accessing the object created
    document.getElementById("demo").innerHTML = fruit.name;
</script>

In this example, there are multiple parameters in the *constructor()* method.

<script>
    class Fruit {
        constructor(fruitName, fruitColor) {
            this.name = fruitName;
            this.color = fruitColor;
            this.taste = "sweet";
        }
    }

    const fruit = new Fruit("apple", "green");

    //accessing the object created
    document.getElementById("demo").innerHTML = 
    "The " + fruitName + " is " + fruitColor + " and " + fruit.taste;
</script>

HEAD OVER TO Multiple-classes.html
---------------------------------------------------------------------