> We will revisit this ^ later...

### Shells

Shell _commands_ can also be edited and run directly in Docable. We will primarily be using Bash shells for this course. In the editor below, type `ls` and run the command to see a list of files used in this workshop.

<!-- 
targets:
    - type: docker
      name: command-example
      image: node:12-buster
-->
```bash|{type:'command', shell:'bash'}

```

We also have basic functionality to validate the output of of commands. For example, modify the following script to print out `goodbye world`:
```bash|{type:'command', failed_when: "stdout.includes('goodbye')", success_message:"Great job 👍", failure_message: "Incorrect output: try 'hello world' instead..."}
echo ""
```

### Variables

Environment variables can also be set and run for bash commands in Docable. The command exampls below run successfully if you have correctly assigned the variable `foo`. If the variables are not set, you should get an error that the variables have not been provided.

```bash|{type:'command', variables: 'foo'}
echo "{{foo}} world"
```

```bash|{type:'command', variables: 'bar'}
echo "hello {{bar}}"
```

### Terminals

Finally, Docable also provides interactive _terminals_ for more extensive tutorial activities. These terminals are also connected to the shell commands and files generated throughout this tutorial. For example, run the command below to write “Hello World!” in /tmp/hello.txt:


```|{type:'command'}
echo "Hello World!" > /tmp/hello.txt
```

Then in the terminal below, type `cat /tmp/hello.txt` to check the result of command cell above:

```|{type:'terminal'}
```

Docable also provides several types of terminals including bash and zsh as well as Evaluate, Print, Loop (REPL) terminals for other programming languages such as node, python, Ruby (irb), and Java (JShell).

## Final Thoughts on Workshops

* To receive credit for completing workshops, you will most likely have to submit screenshots or a pdf of the tutorial (Print > Save As PDF). Each workshop will have specific instructions on what to turn in.
* The academic integrity policy applies to all workshops. Do not work together unless otherwise specified.
* Remember, any workshop content (including this one) is eligible to be on the exam.

### [Bash Shells ⏭️](Shells.md)