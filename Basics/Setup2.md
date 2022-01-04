> We will revisit this ^ later...

### Shells

Shell _commands_ can also be edited and run directly in Docable. We will primarily be using Bash shells for this course. In the editor below, type `ls` and run the command to see a list of files used in this workshop.

<!-- 
targets:
    - type: docker
      name: t1
      image: node:12-buster
    - type: docker
      name: t2
      image: node:12-buster
 -->
```bash|{type:'command', shell:'bash'}

```

We also have basic functionality to validate the output of of commands. For example, modify the following script to print out `goodbye world`:
```bash|{type:'command', failed_when: "stdout.includes('goodbye')", success_message:"Great job 👍", failure_message: "Incorrect output: try 'hello world' instead..."}
echo ""
```

### Variables

Environment variables can also be set and run for bash commands in Docable. Remember the text boxes at the top? The command below will run successfully if you have correctly assigned the variables. Try assigning a string value to `foo` and running the first command:

```bash|{type:'command', variables: 'foo'}
echo "{{foo}} world"
```

If the variables are not set, you should get an error that the values have not been provided. Try running the this command without setting `bar` above:

```bash|{type:'command', variables: 'bar'}
echo "hello {{bar}}"
```

### Terminals

Additionally, Docable also provides full interactive _terminals_ for more extensive tutorial activities. These terminals are also connected to the shell commands and files generated throughout this tutorial. For example, run the command below to write “Hello World!” in /tmp/hello.txt:


```|{type:'command'}
echo "Hello World!" > /tmp/hello.txt
```

Then in the terminal below, type `cat /tmp/hello.txt` to check the result of command cell above:

```|{type:'terminal'}
```

Docable also provides several types of terminals including bash and zsh as well as Evaluate, Print, Loop (REPL) terminals for other programming languages such as node, python, Ruby (irb), and Java (JShell).

### Multi-target Terminals

When working on tutorials with multiple terminals, be careful to observe which commands are run in which target terminal. For example, run the command below will to create a the file `target_test.txt` in terminal **t2**:

```bash|{type:'command', target: 't2'}
touch /tmp/target_test.txt
```

In the terminal below, type the `ls \tmp` command in **t1** below and hit Enter to list all of the files in the current directory you should see that there is no `target_test.txt` available:
```bash|{type:'repl', target: 't1', 'background-color': '#00345c'}
```

However, when you run the `ls \tmp` command in the second terminal, you can find the target test file present on the system:
```bash|{type:'repl', target: 't2', 'background-color': '#013d17'}
```

## Final Thoughts on Workshops

* To receive credit for completing workshops, you will most likely have to submit screenshots or a pdf of the tutorial (`Print > Save As PDF`). Each workshop will have specific instructions on what to turn in.
* The academic integrity policy applies to all workshops. Do not work together unless otherwise specified.
* Remember, any workshop content (including this one) is eligible to be on the exam.

### [Programming Languages ⏭️](Coding.md)