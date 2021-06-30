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

# Type Shapes

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
```

## - ANY type

Variables of type **any** can be assigned to any value and TypeScript won’t give an error if they’re reassigned to a different type later on.

# variable type annotations

# type hints

Found in TypeScript but not JS 
- Interfaces
- Namespaces
- Generics
- Abstract classes
- Data modifiers
- Optionals
- Function overloading
- Decorators
- Type utils
- readonly keyword


# Compiler options
- By using compiler options, you can control how the JavaScript is generated from the source TypeScript. You can set the options either at the command prompt, as you would with many command-line interfaces, or in a JSON file named tsconfig.json.

- Numerous compiler options are available to you. You can find a complete list of options in the tsc command-line interfaces documentation. Here are a few of the most 

    - common options:
    - noImplicitAny
    - noEmitOnError
    - target
    - the directory options


- To control the compilation, you can use compiler options with the tsc command, including:

    - The --noImplicitAny option instructs the compiler to raise errors on expressions and declarations with an implied any type. For example:
        
            tsc utility_functions.ts --noImplicitAny
    
    - The --target option specifies the ECMAScript target version for the JavaScript file. This example compiles an ECMAScript 6-compliant JavaScript file:
            
            tsc utility_functions.ts --target "ES2015"