---
title: Other sources
published: true
---

# Free R resources and tutorials:

There are many functions in R and often more than one way of doing things, so it is impossible to know all of R. Any R course will teach you some aspect of R and for more unique or detailed issues there will be plenty help on-line and in books. On-line forums such as <http://stackoverflow.com/> or <http://stackexchange.com/> are a good way to get different explanations of how to do some more complicated things. In almost all cases, if you run into a problem, someone has already had the same issue, and someone has also solved it. Searching for what you want to do in Google, such as "line plot in R", will give good results.

<br><br>

**Use R help files.** Typing `help.start()` into your Console/code cell will open the R manuals which give you an introduction to R and plenty other information. More often you will need to get more information on a specific function and for that you can use the `help` function or the question mark `?`. For example, if you wanted help on the `plot` function, type `help(plot)` or `?plot`. Try this out yourself. You can use `??` such as `??plot` to search a text string in case there are no help packages set up.[^1]

[^1]: Examples on a how a function can be used and what it produces can normally be run by using the `example` function, such as `example(plot)`

There are a few things to remember when working with R, which when forgotten can easily cause you a lot of headache:

*	**R is case sensitive.** If you get an error message check that there are no capital letters where there should be lower-case letters and vice versa. If you named your dataset *MyData*, then *mydata* or *Mydata* will produce an error reading something like `Error: object 'mydata' not found`. Case sensitivity applies to everything in R, including functions. The square root function is `sqrt` with all small letters and using `Sqrt` will produce an error. Most functions only use small letters.
 
*	**Check that your brackets match up.** All open brackets such as `(`, `{` or `[` should also close with `]`, `}` and `)` respectively. RStudio will help you match brackets by highlighting the closing bracket for all opening brackets and vice versa in the script file. Place the cursor behind any bracket and R will highlight its "partner". If you are missing a bracket R may give the prompt `+` in the console window, indicating that the command is not complete.

* **Check your commas.** All arguments in a function or all elements in a string of numbers/words will have to be separated by commas. For example, to plot two variables *x* and *y* you have to write `plot(x, y)` and excluding the comma will produce and error. To combine numbers 3 and 5 in a vector *z* you have to write `z <- c(3, 5)` and `z <- c(3 5)` will produce an error.

* **Object names.** Object names in R should never include any spaces. You can call your dataset *my_data*, *MyData* or *my.data*, but never *my data*. If you import a dataset that includes spaces in variable names the spaces will automatically be converted to dots such as *my variable* will become *my.variable*. Objects names can also never start with a number or any other symbol than a letter. Variable names such as *25_years* or *1.year* are not allowed but *years_25* or *new.year* are. Most symbols such as % / \ ( ) are also not allowed in object names.

*	**Backslash and forward slash.** Windows uses the backslash `\` for paths to directories (folders), but R uses forward slash `/` or `\\` for paths to directories. In R `\` has a different meaning; it is an escape character.

*	**Assignment operators.** The symbol `<-` is used in R as an assignment operator -- it assigns values to names, e.g. `a <- 20` assigns the value 20 to the letter *a*. You can also use `=` as an assignment operator, but the more common symbol for assignment is `<-`. The symbol `=` is also used to give values to arguments in functions, such as `plot(1, 2, xlab="My x axis", ylab="My y axis")`. But note you cannot use `ylab <- "My y axis"`. The symbol `==` has a completely different meaning and is used for logical comparison, such as `a==20` will test whether *a* is equal to 20. You can use `help("==")` or `?"<-"` to see more.

#Resources

There is an extensive amount of resources about R on the internet, just Google "R books" and you will find plenty. Here is a list of some helpful materials:

* RStudio cheat sheets (multilingual) <https://www.rstudio.com/resources/cheatsheets/>

* An Introduction to R <http://cran.r-project.org/manuals.html>

* R for Beginners <https://cran.r-project.org/doc/contrib/Paradis-rdebuts_en.pdf>

* Cookbook for R <http://www.cookbook-r.com/>

* R in Action <https://www.manning.com/books/r-in-action-second-edition> and the related Quick-R website <http://www.statmethods.net>

* Advanced R <http://adv-r.had.co.nz/> by Hadley Wickham, the Chief Scientist at RStudio

* Code Academy <https://www.codecademy.com/learn/learn-r>
