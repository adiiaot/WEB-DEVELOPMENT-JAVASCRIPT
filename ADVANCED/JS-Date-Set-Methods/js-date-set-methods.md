# JAVASCRIPT DATE SET METHODS
The following methods allow us to get Date values such as year, month, day and more.

* Method   - * Description
* *Date.setTime()* -  Sets the date to the time represented by a number of milliseconds since January 1, 1970.

* *Date.setFullYear()* - Sets the year for a specified date.

* *Date.setMonth()* - Sets the month for a specified date.

* *Date.setDate()* - Sets the day of the month for a specified date.

* *Date.setHours()* - Sets the hour for a specified date.

* *Date.setMinutes()* - Sets the minutes for a specified date.

* *Date.setSeconds()* - Sets the seconds for a specified date.

* *Date.setMilliseconds()* - Sets the milliseconds for a specified date.
---------------------------------------------------------------------


# *Date.setTime()* METHOD
The *Date.setTime()* methods sets the date to the time represented by a number of milliseconds since January 1, 1970.

In this example, we get the milliseconds elapsed between January 1, 1970 and November 21, 2023.

Next, set the date of *date2* using that milliseconds.

Then we added 86400000 (1 day) milliseconds.

<script>
    const date1 = new Date("Nov 21, 2023");
    const date2 = new Date():
    date2.setTime(date1.getTime() + 86400000); //get the milliseconds and add 1 day 

    document.getElementById("demo").innerHTML = date2;
</script>

---------------------------------------------------------------------


# *Date.setFullYear()* METHOD
This sets the year for a specified date.

<script>
    const date = new Date();
    date.setFullYear("2023");
</script>

---------------------------------------------------------------------


# *Date.setMonth()* METHOD
This sets the month for a specified date. The index 0 represents January, 1 represents Febuary, and so on.

<script>
    const date = new Date();
    date.setMonth(5); //sets month to June
</script>

---------------------------------------------------------------------


# *Date.setDate()* METHOD
This method sets the day of the month for a specified date.

<script>
    const date = new Date();
    date.setDate(4); 
</script>

---------------------------------------------------------------------


# *Date.setHours()* METHOD
This method sets the hours for a specified date.

<script>
    const date = new Date();
    date.setHours(8);
</script>

---------------------------------------------------------------------


# *Date.setMinutes()* METHOD
This method sets the minutes for a specified date.

<script>
    const date = new Date();
    date.setMinutes(30);
</script>

---------------------------------------------------------------------


# *Date.setSeconds()* METHOD
This method sets the seconds for a specified date.

<script>
    const date = new Date();
    date.setSeconds(50);
</script>

---------------------------------------------------------------------


# *Date.setMilliseconds()* METHOD
This method sets the milliseconds for a specified date.

<script>
    const date = new Date();
    date.setMilliseconds(450);
    date.getMilliseconds(); //get milliseconds
</script>