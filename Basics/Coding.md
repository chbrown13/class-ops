# Programming Languages

> "You may not get to choose what programming language you use for your project, but it may be the most important choice there is. Programmers have argued about which language is best for as long as there have been programmers. In my experience, it makes a lot less difference than most people think…" - [Greg Wilson](https://buildtogether.tech/tooling/#programming-language)

One of the first things you need to know to be a successful software engineer is a programming language. Developers should also be able to quickly learn new programming languages and transfer knowlede between languages, which can be [very difficult to do](http://nischalshrestha.me/docs/cross_language_interference.pdf). Run the following code scripts to print `hello world!` in various programming languages:

```js |{type:'script'}
    console.log( "hello world!" );
```

```python |{type:'script'}
    print("hello world!")
```

```ruby |{type:'script'}
    print 'hello world!'
```
```java |{type:'script'}
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("hello world!");
    }
}
```

## Write-Compile-Execute

In general, all of coding can be summed up by the **Write -> Compile -> Execute** process:

### Write
Also known as "Code" (code-compile-execute), this phase involves giving instructions to the computer by creating a program with source code. This program is:
– Written in a programming language (i.e. Java)
– Human-readable
– Written using a text editor or integrated development environment (IDE)

### Compile
Compilation translates the program from one language to another that can be understood by hardware. **Bytecode** is an intermediate language that has been compiled from source code and translated into low-level code. Some programming languages have distinct compilation steps (i.e. Java) while others compile during execution (i.e. Python). 

### Execution
The computer or a virtual machine reads and acts on the translated instructions from the written program. When either Compilation or Execution fails, return to Writing to update the source code.

## Shell Programming

A **Read-Eval-Print Loop (REPL)** is an interactive interpreter for programming languages. This concept originated with LISP, but many other languages today (Python, Ruby, JavaScript, Haskell, etc.) use REPL's to provide interactive programming language environments that bypass the compile stage of the write-compile-execute cycle. REPLs are useful for simple experimentation and developing quick functions with languages.

There are 4 components to REPL environments:

    * _Read_ reads in input from the keyboard
    * _Eval_ evaluates code passed to it
    * _Print_ formats and displays the output
    * _Loop_ continues the three previous commands until the REPL is terminated

## Activity

Below are four REPL environments for different programming languages (Python, JavaScript, Ruby, and Java). Complete the program below in **one** of the terminals below. When you are finished, take a screenshot with the completed code and the output in the REPL you selected. Save with the name "fizzbuzz" (as a .jpg, .png, or .pdf). You can submit one screenshot or two separate for code (fizzbuzz_code) and output (fizzbuzz_output). If you are not familiar with any of these languages, complete the program in the language of your choice and save it in a source code file (i.e. `file.c` for C programs).

> **Fizz Buzz**
> 
> Fizz buzz is a classic [children's game](https://en.wikipedia.org/wiki/Fizz_buzz) and [programming challenge](https://leetcode.com/problems/fizz-buzz/). Write a program that prints each number from 1 to 20 separated by a space. If the number is divisible by 3, print `Fizz` instead. If the number is divisible by 5, print `Buzz` instead. And if the number is divisible by 3 and 5, then print `FizzBuzz`. This is a simple activity to practice shell programming- you are not expected to come up with the most efficient solution and you will not be graded on correctness. Your program must at least contain some type of loop structure, conditional statements, and print statements.

```|{type:'terminal', command: 'node'}
```

```|{type:'terminal', command: 'python'}
```

```|{type:'terminal', command: 'irb'}
```

```|{type:'terminal', command: 'jshell'}
```

* Remember to take your screenshot!

### [**Bash Shells** ⏭️ ](Shells.md)
