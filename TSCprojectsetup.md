# Generate a tsconfig.json file
CLI: 
            
            tsc --init
# config tsconfig.json file

- In the file 
    - In the tsconfig.json file, look for the target option and change it to "ES2015".
    - Update the tsconfig.json file so that the compiler saves all JavaScript files to a new folder.
        
        - a. On the Explorer pane, create a new folder in your project called build.
        - b. In the tsconfig.json file, look for the outDir option, remove the comment, and set the parameter to build.

- Save the tsconfig.json file.
- At the command prompt, **enter tsc**. This reads the jsconfig.json file and resets the options for the project.