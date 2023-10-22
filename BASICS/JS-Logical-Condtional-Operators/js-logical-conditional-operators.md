# JAVASCRIPT LOGICAL OPERATORS
Logical Operators are commonly used with *Booleans*.

When they are used with Boolean (logical) values, they return a Boolean value.

In JavaScript, there are 3 logical operators:

1. Logical AND  &&   used as (expression1 && expression2)
2. Logical OR   ||   used as (expression1 || expression2)
3. Logical NOT  !    used as (expression1 ! expression2)

# LOGICAL AND (&&)
The logical AND (&&) operator returns *true* if BOTH OPERANDS (which are expressions) are *true*.

<script>
    true && true; //returns true
    true && false; //returns false
    3 == 3 && 4 == 4; //returns true
    3 == 4 && 4 == 4; //returns false
    5 > 3 && 4 < 6; //returns true
    3 > 5 && 6 < 4; //returns false
</script>

HEAD OVER TO Logical AND (logical-AND.html) TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------

# LOGICAL OR (||)
The logical OR (||) operator returns *true* if EITHER of the operand is *true*.

<script>
    true || true; //returns true
    true || false; //returns true
    false || false; //returns false
    2 == 2 || 2 == 2; //returns true
    1 == 2 || 2 == 3; //returns false
    10 > 5 || 5 > 10; //returns true
    10 < 5 || 5 > 10; //returns false
</script>

HEAD OVER TO Logical OR (Logical-OR.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# LOGICAL NOT (!)
The logical NOT (!) operator returns *true* if the operand is NOT TRUE.

<script>
    !(true); //returns false
    !(false); //returns true
    !(1 == 1); //returns false
    !(1 > 2); //returns true
</script>

HEAD OVER TO Logical-NOT (logical-NOT.html) TO SEE THE OUTPUT OF THIS CODE.
---------------------------------------------------------------------

* Now how do we use this logical operator?

# USING LOGICAL OPERATORS WITH CONDITIONAL STATEMENTS

Logical Operators are commonly used with *conditional statements*

The example below, shows how to use a logical operator in an *if* statement.

<script>
    if (3 == 3 && 4 == 4) {
        document.write("This condition is true");
    }

    if (3 == 3 && 3 == 4) {
        document.write("I will not be printed because this condition is false");
    }

</script>

HEAD OVER TO Sample-FIle (Using-Logical.html) TO SEE THE OUTPUT OF THIS CODE
---------------------------------------------------------------------


# JAVASCRIPT CONDITIONAL (TERNARY) OPERATOR
The conditional or the ternary operator is the only operator that takes three operands.

condition ? value1 : value2

if the *condition* is true, the operator returns *value1*, otherwise, it returns *value2*.

This is commonly used with a variable.

<script>
    var testScore = 80;
    var testResult = (testScore > 75) ? "passed" : "failed";
    document.getElementById("demo").innerHTML = testResult;
</script>

HEAD OVER TO Sample-File (testresult.html) TO SEE THE OUTPUT OF THIS CODE.

Since the *testScore* is more than 75, then the value "passed" will be assigned to the *testResult* variable.

If the *testScore* is less than 75, the value "failed" will be assigned instead.

Want to give it a try?

Use the code below and replace it with the <script> code in "testResult.html" file to see your output

<script>
    var testScore = 80;
    var testResult = (testScore < 75) ? "passed" : "failed";
    document.getElementById("demo").innerHTML = testResult;
</script>