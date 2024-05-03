# Step 1 Check Variables

In the code we add 3 examples for it work properly or not
```
function printVariables() {
    // Define some variables
    var a = 5;
    var b = "Hello";
    var c = { name: "John", age: 30 };

    // Get all variable names in the current scope
    var variableNames = Object.keys(this);

    // Print each variable and its value
    variableNames.forEach(function(name) {
        console.log(name + ": " + this[name]);
    }, this);
}
```

### Method How to work (use)
paste it on the console : 
> + Chrome: Cmd + Option + J on a Mac, or Ctrl + Shift + J on Windows
> + Firefox: Cmd + Option + K on a Mac, or Ctrl + Shift + J on Windows
> + Edge: F12 to access the Developer Tools, then navigate to the Console tab

And Run this code 
```
printVariables();
```
