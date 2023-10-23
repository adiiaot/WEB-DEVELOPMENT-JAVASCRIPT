# WHAT IS AN OBJECT?
An *object* is a collection of related data and/or functionality.

Most of the time, creating an *object* begins with defining a variable.

<script>
    var person = {
        fullName: "Adii Aot",
        age: 18,
        hobbies: ["coding", "gaming", "playing chess"],
        isSingle: true
    }
</script>

As you can see, the syntax of an object is pretty simple.

The *person* object contains "properties".

Each properties has a *name* (e.g fullName, age) and a *value* (e.g "Adii Aot", 18).

"Properties" are seperate by commas (,).

The *name* and *value* pair are seperated by a colon (:).
---------------------------------------------------------------------

# METHODS IN AN OBJECT
An object can also contain *function* (methods).

<script>
    var person = {
        fullName: "Adii Aot",
        age: 18,
        showName: function(){
            alert(this.fullName);
        },
        showAge: function(){
            alert(this.age);
        }
    }
</script>

*NOTE! An object is a collection of properties and/or methods.
---------------------------------------------------------------------

# ACCESSING OBJECT'S PROPERTIES

There are two ways to access an object's members (properties and methods).

* THE DOT NOTATION
The Dot Notation uses a dot (.) to access an object's members.

First write the variable, then the name of a property or method.

<script>
    person.name;
    person.age;
    person.hobbies[0];
</script>

HEAD OVER TO Using-Dot-Notation (Dot.html) TO SEE THE OUTPUT AND HOW THIS IS USED IN A CODE
------
------

* THE BRACKET NOTATION
We can also use *square brackets* to access an object's members.

<script>
    person["fullName"];
    person["age"];
    person["hobbies"][0];
</script>

HEAD OVER TO Using-Brackets-Notation (Brackets.html) TO SEE HOW THIS CODE IS BEING USED
------
------

* THE *this* KEYWORD
You may have noticed the *this* keyword in one of our examples. This may look strange, but don't worry, it's easy. for realllll.

The *this* keyword refers to the current object.

<script>
    var person = {
        fullName: "Adii Aot",
        age: 18,
        showDetails: function(){
            alert(this.fullName + " is " + this.age + " years old.")
        }
    };
</script>

HEAD OVER TO Using-This-Keyword (this.html) TO SEE HOW THIS CODE IS BEING USED.

In this case, *this* is equivalent to the *person* object.
---------------------------------------------------------------------


# AN OBJECT IN AN OBJECT.

Yes, it is possible to put objects inside an object.

<script>
    var animals = {
        lion: {
            color: "yellow",
            food: "meat"
        },
        tiger: {
            color: "red",
            food: "fowl"
        }
    }

    document.write(animals.lion.color);
</script>
HEAD OVER TO Objects-in-Objects (objects.html) TO SEE HOW THIS CODE IS BEING USED.

As you may have noticed we accessed the *color* property using the "animals.lion.color".