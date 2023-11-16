# JAVASCRIPT DATES
The *Date* object allows us to work with dates.

# THE *Date()* CONSTRUCTOR
The *new Date()* constructot returns a Date object

There are 4 basic forms of the date constructor.

* new Date()
* new Date(milliseconds)
* new Date(dateString)
* new Date(year, monthIndex, day, hours, minutes, seconds, milliseconds)

# *new Date()*
*new Date()* creates a Date object representing the current DATE and TIME.

<script>
    var date = new Date();
</script>

HEAD OVER TO Date.html
---------------------------------------------------------------------


# *new Date(milliseconds)* 
*new Date(milliseconds)* creates a Date object representing the *date* milliseconds since *January 1, 1970.

For example, the date below is equivalent to 86, 400,000 milliseconds (1 day) since January 2, 1970.

<script>
    var date = new Date(86400000);
    document.write(date);
</script>

HEAD OVER TO Date-milliseconds.html
---------------------------------------------------------------------


# *new Date(dateString)*
*new Date(dateString)* creates a Date object representing the *date* from a *date string*.

<script>
    var date = new Date("November 16, 2023");
    document.write(date);
</script>

HEAD OVER TO Date-strings.html
---------------------------------------------------------------------

Date strings will be discussed further in the next section.


# *new Date(year, monthIndex, ...)*
The *new Date(year, monthIndex, ...)* creates a Date object from 7 parameters:

* years - integer representing the year.
* monthIndex - integer representing the month 0 is for January and 11 is for December
* day -integer representing the day, default is 1.
* hours - integer representing the hour of the day, default is 0 (midnight).
* minutes - integer representin the minutes, default is 0
* seconds - integer representing the seconds, default is 0
* milliseconds - integer representing milliseconds, default is 0.

All these parameters are optional.

* 7 parameters specify year, monthIndex, day, hours, minutes, seconds, milliseconds:

<script>
    var date = new Date(2023, 11, 16, 18, 20, 20, 0);
    document.write(date);
</script>

* 6 parameters specify year, monthIndex, day, hours, minutes, seconds:

<script>
    var date = new Date(2023, 11, 16, 18, 20, 20);
    document.write(date);
</script>

* 5 parameters specify year, monthIndex, day, hours, minutes:

<script>
    var date = new Date(2023, 11, 16, 18, 20);
    document.write(date);
</script>

* 4 parameters specify year, monthIndex, day, hours:

<script>
    var date = new Date(2023, 11, 16, 18);
    document.write(date);
</script>

* 3 parameters specify year, monthIndex, day:

<script>
    var date = new Date(2023, 11, 16);
    document.write(date);
</script>

* 2 parameters specify year, monthIndex:

<script>
    var date = new Date(2023, 11);
    document.write(date);
</script>

* 1 parameters will use the *new Date(milliseconds)*:

<script>
    var date = new Date(864000000);
    document.write(date);
</script>

