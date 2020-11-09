# Code Best Practice


## Code Smells Summary
##### "Code smell is an evocative term for that vague feeling of unease we get when reading certain bits of code. It's not necessarily wrong, but neither is it obviously correct. We may be reluctant to work on such code, because past experience suggests it's going to be fiddly and bug-prone. In contrast, there's another type of code that just feels good to read and work on." - [Jenny Bryan](https://github.com/jennybc/code-smells-and-feels#:~:text=GitHub%3A%20%40jennybc%20%22Code%20smell%22%20is%20an%20evocative%20term,suggests%20it%27s%20going%20to%20be%20fiddly%20and%20bug-prone.)

###  Refractoring 
* Making code easier to understand and modify without changing it's behaviour

## Do's
### Make a README 
  * Here is the GDS [guidance on writing READMEs](https://gds-way.cloudapps.digital/manuals/readme-guidance.html#writing-readmes)
  * Helps the user: 
      * Understand what the project is
      * Learn how to use the project
### Comment all code 
  * Explain _**what**_ it is doing and _**why**_ it is doing it
  * This will make it easier for you and other users to know what the code is for
  
###  Lint your code
  * **Linting**: The automated checking of your source code for programmatic and stylistic errors
  * [Lintr](https://github.com/jimhester/lintr) checks your code for style, syntax errors and possible semantic issues
  
### Use meaningful variable and function names
  * `height_in_metres()` is better than `converter()` for a function that converts height into metres 
  * This makes it more obvious what your code is doing
  * Makes your code more readable
  * Use a readable [case style](https://medium.com/better-programming/string-case-styles-camel-pascal-snake-and-kebab-case-981407998841) 
  
### Avoid absolute filepaths
  * You could either:
      * Use the library [`here()`](https://github.com/krlmlr/here)
      * Work within an [R project](https://support.rstudio.com/hc/en-us/articles/200526207-Using-Projects)
      * Use `getwd()` & `setwd()` 
      
### Keep your scripts to a reasonable length (ideally less than 250 lines)
  * This keeps them more manageable
  * Break up and `source()` sections like data processing, and variable or function assigning
  
### Uncommenting code
  * Don't rely on (un)commenting code to change behaviour   
  * Remove any just-in-case code you don’t actually need
  
### Avoid nested `for` loops/`ifelse`
  * Use casewhen()
  * Every `if` does not need an `else` if you `stop()` or `return()`
  
### Use Functions
  * A few little functions are better than one massive one
  * This includes small, well named, helper functions
  
### Proper functions
  * Use the built in proper functions to simplify 
  
### Stop early
  *  Move quick `stop()`s and `return()`s to the top of the function
  
### Use `switch()`
  * `switch()` is great for running different logic based on a string
  
### Put your contact details somewhere



###### Author: rhiannon.batstone@nrscotland.gov.uk
