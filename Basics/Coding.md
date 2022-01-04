# Programming Languages

> "You may not get to choose what programming language you use for your project, but it may be the most important choice there is. Programmers have argued about which language is best for as long as there have been programmers. In my experience, it makes a lot less difference than most people think…" - [Greg Wilson](https://buildtogether.tech/tooling/)

One of the first things you need to know to be a successful software engineer is a programming language. Learning a coding languages is important, however just as important may be the ability to apply concepts and learn new programming languages on the fly, which is [very difficult to do](http://nischalshrestha.me/docs/cross_language_interference.pdf). In general, no matter what programming language you choose all of coding can be summed up by the process *Write-Compile-Execute*.

### Write
This phase involves giving instructions to the computer by creating a program with source code. This code is:
– Written in a programming language (i.e. Java)
– Human-readable
– Written using a text editor or integrated development environment (IDE)

### Compile
Compilation translates the program from one language to another that can be understood by hardware. **Bytecode** is an intermediate language that has been compiled from source code and translated into low-level code. Some programming languages have distinct compilation steps (i.e. Java) while others compile during execution (i.e. Python). 

### Execution
The computer or a virtual machine reads and acts on the translated instructions from the written program. When either Compilation or Execution fails, return to Writing to update the source code.

Run the following code snippets to print `hello world!` in various programming languages with Docable:

```js |{type:'script'}
console.log( "hello world!" );
```

```python |{type:'script'}
print("hello world!");
```

```java |{type:'script'}
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("hello world!");
    }
}
```

```ruby |{type:'script'}
print 'hello world!'
```

Complete the basic coding tasks to practice using programming concepts in different languages:


```python | {type: 'script', failed_when: "stdout.includes('0\n')", success_message:"Nice, you run this command successfully!", failure_message: "Try again"}

```

#### [**Bash Shells** ⏭️ ](Shells.md)
