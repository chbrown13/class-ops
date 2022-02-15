# Software Metrics

This activity will allow you to practice using various tools to calculate various code metrics discussed in class. To submit this assignment, answer all of the questions below in a .txt or .pdf file to submit on Canvas. Pay attention to activities completed on your local machine (_you should have installed a package manager on your machine in the previous notebook_) or on Docable.

### Exercise: Lines of Code

`sloc` is a basic tool that counts [source lines of code](https://www.npmjs.com/package/sloc). Install the `sloc` package on to your system:

`npm install -g sloc`

> Alternatively, you can use Count Lines of Code (`cloc`) on Chocolatey: [https://chocolatey.org/packages/CLOC](https://chocolatey.org/packages/CLOC)

To run these tools, simply open a command-line and type:

```cloc <file-name>``` / ```sloc <file-name>``` 

to count the number of lines in a specific file or

```sloc .``` / ```cloc .``` 

to count the number of lines for all of the files in the current directory.

More details are available using `sloc -h` or `cloc -help`. Use one of the lines of code counting tool to answer the following questions:

1. How many total lines of code are in your pair programming workshop repository?
