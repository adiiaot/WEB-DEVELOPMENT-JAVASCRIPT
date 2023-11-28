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


# METHODS IN CLASSES
Just like in a regular object, you can add functions (methods) to a class.

In this example, the *showInfo()* function is added to the class:

<script>
    class Fruit {
        constructor(fruitName, fruitColor){
            this.name = fruitName;
            this.color = fruitColor;
            this.taste = "sweet";
        }

        showInfo() {
            document.getElementById("demo").innerHTML = 
            " The " + this.name + " is " + this.color + " and " + this.taste;
        }
    }

    const fruit = new Fruit("Apple", "green");
    fruit.showInfo();
</script>

Then, we call the function after the class has been initialized:

HEAD OVER TO Method-class.html
===============
===============

We can also add PARAMETERS to the function.

The parameters should go inside the parantheses..

<script>
    class Fruit {
        constructor(fruitName, fruitColor){
            this.name = fruitName;
            this.color = fruitColor;
            this.taste = "sweet";
        }

        showMessage(text) {
            document.getElementById("demo").innerHTML = text;
        }
    }

    const fruit = new Fruit("Apple", "green");
    fruit.showMessage("I love Fruits!");
</script>

=====================================================================


# STATIC METHODS
Static methods are called without initializing their class.

A static method (*sayHello()*) cannot be called by the object (*myFruit()*), but it can be called using the class (*Fruit*).

<script>
    class Fruit {
        constructor(fruitName, fruitColor){
            this.name = fruitName;
            this.color = fruitColor;
        }
        static sayHello(text){
            return text;
        }
    }

    document.getElementById("demo").innerHTML = 
    Fruit.sayHello("Making Progress with Fruits!");
</script>

HEAD OVER TO Static-methods.html
---------------------------------------------------------------------


# CLASS INHERITANCE
Class inheritance is a way for a class to inherit all the properties and methods of another class.

This way, we create new functionality on top of the existing.

The *Animal* class below can be used to tell that an animal can walk.

<script>
    class Animal {
        constructor(animalName){
            this.name = animalName;
        }

        walk(){
            return this.name + " walks";
        }
    }
</script>

Let's say we want to create another class called *Cat*.

Since a cat is also an animal, it's a good idea to have access to all the properties and methods of the *Animal* class.

The syntax to inherit a class is:

<script>
    class Cat extends Animal
</script>

Here is the full example:

<script>
    class Animal {
        constructor(animalName){
            this.name = animalName;
        }

        walk(){
            return this.name + " walks";
        }
    }

    class Cat extends Animal {
        constructor(animalName){
            super(animalName);
        }

        speak(){
            return this.name + " meows";
        }
    }

    const cat = new Cat("mingming");
    document.getElementById("demo").innerHTML =
    cat.walk() + " and " + cat.speak();
</script>

HEAD OVER TO Class-inheritance.html
==============
==============

Notice that we used the *super()* method in the constructor of the *Cat* class.

The *super()* method is used to call the parent's class (Animal) constructor to get access to its properties and methods.

Because of that, we were able to use both *walks()* and *speak()* methods by just using the *cat* object.