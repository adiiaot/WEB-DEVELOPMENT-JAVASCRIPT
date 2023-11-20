# JAVASCRIPT DATE GET METHODS
The following methods are used to get information from a *Date* object.

* *Date.now()* - Returns the number of milliseconds elapsed since January 1, 1970.

* *Date.getFullYear()* - Returns the year of the specified date.

* *Date.getMonth()* - Returns the month index (0-11) of the specified date.

* *Date.getDate()* - Returns the day of the month for the specified date.

* *Date.getDay()* - Returns the day index of the week for the specified date.

* *Date.getHours()* - Returns the hours of the specified date.

* *Date.getMinutes()* - Returns the minutes in the specified date.

* *Date.getSeconds()* - Returns the seconds in the specified date.

* *Date.getMilliseconds()* - Returns the milliseconds in the specified date.

* *Date.getTime(givenDate)* - Returns the time elapsed between January 1, 1970 and the *givenDate* 
---------------------------------------------------------------------


# *Date.now()* METHOD
The *Date.now()* method returns the number of milliseconds elapsed since January 1, 1970.

<script>
    const now = Date.now();
    document.write(now);
</script>

HEAD OVER TO Date-now.html
---------------------------------------------------------------------


# *Date.getFullYear()* METHOD
The *Date.getFullYear()* method returns the year of the specified date.

<script>
    const date = new Date();
    const year = Date.getFullYear();
</script>

HEAD OVER TO Date-fullyear.html
---------------------------------------------------------------------


# *Date.getMonth()* METHOD
The *Date.getMonth()* method returns the month index of the specified date 0 is January and 11 is December.

<script>
    const date = new Date();
    const month = date.getMonth();
</script>

HEAD OVER TO Date-month.html
---------------------------------------------------------------------


# *Date.getDate()* METHOD
The *Date.getDate()* method returns the day of the month for the specified date.

<script>
    const date = new Date();
    const day = date.getDate();
</script>

HEAD OVER TO Date-getDate.html
--------------------------------------------------------------------


# *Date.getDay()* METHOD
The *Date.getDay()* method returns the day index of the week for the specified date. 0 is Sunday and 6 is Saturday.

<script>
    const date = new Date();
    const day = date.getDay();
</script>

HEAD OVER TO Date-day.html
---------------------------------------------------------------------


# *Date.getHours()* METHOD
This returns the hour of the specified date.

<script>
    const date = new Date();
    const hours = date.getHours();
</script>

HEAD OVER TO Date-hours.html
---------------------------------------------------------------------


# *Date.getMinutes()* METHOD
This returns the minutes in the specified date.

<script>
    const date = new Date();
    const minutes = date.getMinutes();
</script>

HEAD OVER TO Date-minutes.html
---------------------------------------------------------------------


# *Date.getSeconds()* METHOD
This returns the seconds in the specified date.

<script>
    const date = new Date();
    const seconds = date.getSeconds();
</script>

HEAD OVER TO Date-seconds.html
--------------------------------------------------------------------


# *Date.getMilliseconds()* METHOD
This returns the milliseconds in the specified date

<script>
    const date = new Date();
    const milliseconds = date.getMilliseconds();
</script>


HEAD OVER TO Date-milliseconds.html
---------------------------------------------------------------------


# *Date.getTime(givenDate) METHOD
This returns the time elapsed between January 1, 1970 and the givenDate.

<script>
    const date = new Date();
    const milliseconds = date.getTime(date);
</script>

HEAD OVER TO Date-givenTime.html