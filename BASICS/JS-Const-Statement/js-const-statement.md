# JAVASCRIPT *const* STATEMENT
The *const* keyword is another way to declare variables.

The *let* and *const* statements behave the same way.

The only difference are the following:

# THE *const* STATEMENT

Variables declared using *const* statement can NOT be *reassigned* and can NOT be *redeclared*.

For example, reassigning a *const* variable will throw an error.

We can see the error report using the try...catch statement.

<script>
    try {
        const x = 3; 
        x = 5; // throws an error
    }
    catch(error){
        document.write(error);
    }
</script>

HEAD OVER TO Re-assigning.html 

Re-declaring will also not work:

<script>
    const x = 5;
    const x = 10; //this will fail
</script>

<script>
    const x = 5;
    var x = 10; //this will fail
</script>