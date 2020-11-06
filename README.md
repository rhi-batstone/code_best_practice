

### Do's
* Make a README
* Comment all code explaining what it is doing
* Lint your code
* Put your contact details somewhere
* Use meaningful variable names
* Avoid absolute filepaths

## Code Smells
##### "Code smell is an evocative term for that vague feeling of unease we get when reading certain bits of code. It's not necessarily wrong, but neither is it obviously correct. We may be reluctant to work on such code, because past experience suggests it's going to be fiddly and bug-prone. In contrast, there's another type of code that just feels good to read and work on." - [Jenny Bryan](https://github.com/jennybc/code-smells-and-feels#:~:text=GitHub%3A%20%40jennybc%20%22Code%20smell%22%20is%20an%20evocative%20term,suggests%20it%27s%20going%20to%20be%20fiddly%20and%20bug-prone.)

###  Refractoring 
* Making code easier to understand and modify without changing it's behaviour



### Tips from [Jenny Bryan's Code Smells talk](https://www.youtube.com/watch?v=7oyiPBjLAWY)
1. Uncommenting code
    * Don't rely on (un)commenting code to change behaviour
    * Remove any just-in-case code you don’t actually need
2. Avoid nested `for` loops/`ifelse`
    * Use casewhen()
    * Every `if` does not need an `else` if you `stop()` or `return()`
3. Use Functions
    * A few little functions are better than one massive one
    * This includes small, well named, helper functions
4. Proper functions
    * Use the built in proper functions to simplify 
5. Stop early
    *  Move quick `stop()`s and `return()`s to the top of the function
6. Dealing with `class()`
    * If your conditions deal with class, it's time to get object-oriented (polymorphism)
7. `switch()`
    * Use `switch()` is great for running different logic based on a string


### List of Code Smells: 
* Duplicated Code
* Long Method
* Large Class 
* Long Parameter List
* Divergent Change 
* Shotgun Surgery
* Feature Envy 
* Data Clumps
* Primitive Obsession 
* Switch Statements
* Parallel Inheritance Hierarchies 
* Lazy Class
* Speculative Generality 
* Temporary Field
* Message Chains 
* Middle Man
* Inappropriate Intimacy 
* Alternative Classes with Different Interfaces
* Incomplete Library Class 
* Data Class
* Refused Bequest 
* Comments

Author: "rhiannon.batstone@nrscotland.gov.uk"
