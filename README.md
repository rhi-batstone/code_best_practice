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
   * Explain what it is doing
   
###  [Lint](https://github.com/jimhester/lintr) your code
   * **Linting**: The automated checking of your source code for programmatic and stylistic errors.
   
### Put your contact details somewhere
   * So 
### Use meaningful variable names
   * 
### Avoid absolute filepaths
   * You could either:
         1. Use the library [`here()`](https://github.com/krlmlr/here)
         2. Work within an [R project](https://support.rstudio.com/hc/en-us/articles/200526207-Using-Projects)
         3. Use `getwd()` & `setwd()` 
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
### `switch()`
   * Use `switch()` is great for running different logic based on a string


Author: "rhiannon.batstone@nrscotland.gov.uk"
