- Typescript was created in 2012 by Microsoft 

    - adds Types to Javascript 
        - type system
                - spot potential bugs
                -clarify structure of code
                - helps in refractor of code
                - arrow functions and classes added to typescript before even added to Javascript itself
- file exension is .ts
- typescript is ran through a transcompiler that checks that code adheres to typescript standards. 
    - will display errors when it does not 
- TypeScript is a superset of javascript 

# Type Interfaces

- when a variable is declared in TypeScript
that variable can never be reassigned a value of a different data type. 

- TypeScript recognizes JS bult in primitive data types:
    - boolean
    - number 
    - null
    - string
    - undefined

# Type Shades

An objects shape describes what properties and methods it does or doesnt contain. 

for example all strings ae known to have the property type of .length and .toLowerCase() method 

    ``` javascript
    "OH".length; // 2
    "MY".toLowerCase(); // "my"
    ```

- the **tsc** command will let you know if your code tries to access properties and methods that dont exist 

example 

``` javascript
"MY".toLowercase();
// Property 'toLowercase' does not exist on tyoe "my"
// Did you mean "toLowerCase"