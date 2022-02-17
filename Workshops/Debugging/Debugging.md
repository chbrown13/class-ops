# Debugging

**Debugging** is the process of finding and removing errors from code. These include _syntax errors_ where a programming language is misused (usually caught by the compiler), _logic errors_ where the code is syntactically correct but there is incorrect output, and _runtime errors_ when the program stops during execution. Research shows debugging is one of the most time-consuming activities for developers and one of the most expensive processes of software engineering.[^1]

Tips for debugging:
- Do not make random or extensive changes to the program! Instead, examine the code to figure out what went wrong.
- Think before you change anything
- Figure out why it went wrong
- Always address the first compiler error listed before addressing the other errors.
- Always recompile after making changes to code because fixing one error will often fix other errors as well.

## 📝 Activity: Debugging Practice

Check out the following code samples below. Debug the programs below to find any errors. When you are finished, copy the fixed files and store them locally on your own machine.

## Debugging Tools

To improve debugging for software engineers, a variety oftools have been developed to support debugging activities. Most IDEs, such as [VS Code](https://code.visualstudio.com/docs/editor/debugging) and [Eclipse](https://www.eclipse.org/community/eclipse_newsletter/2017/june/article1.php), include built-in debuggers to help users find and fix errors in their code. Below are several more examples of debugging tools:

### GDB

[GDB](https://www.sourceware.org/gdb/) (Gnu Project debugger) is a command-line debugging tool that supports a variety of languages. This system is able to do four main activities to help developers catch bugs in the act: 1) Start your program, specifying anything that might affect its behavior; 2) Make your program stop on specified conditions; 3)Examine what has happened, when your program has stopped; and 4)  Change things in your program, so you can experiment with correcting the effects of one bug and go on to learn about another. 

### Valgrind

[Valgrind](https://valgrind.org/) is a dynamic debugging tool that inserts error-checking instructions as it runs your code. This will cause overhead when running your program, but is automatically able to detect many memory management and threading bugs that often cannot be found statically. You can also use Valgrind to build new tools. Valgrind is also a dynamic analysis instrumentation framework for building new tools. The default tool is `memcheck`, which is able to find errors with heap-allocated memory, out-of-bounds access to memory, leaked memory, and uninitialized memory. To run it, you would use the following command:

```bash
valgrind --tool=memcheck ./program
```




## 📝 Activity: Debugging Tools



[^1] [An Exploratory Study of Debugging Episodes](https://arxiv.org/pdf/2105.02162.pdf)