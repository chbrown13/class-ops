<!-- 
targets:
    - type: docker
      name: t1
      image: node:12-buster
    - type: docker
      name: t2
      image: node:12-buster
 -->



> We will revisit this ^ later...

### Shells

Shell _commands_ can also be edited and run directly in Docable. We will primarily be using Bash shells for this course. In the editor below, type `ls` and run the command to see a list of files used in this workshop.

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

cells can specify the target they should execute in using a `target` property. For example, if we create a command cell using this markdown below, the command will run in **t2**.

    ```bash|{type:'command', target: 't2'}
    touch /tmp/hello_world
    ```

You can also see the selected target in the rendered view next to the cell:

```bash|{type:'command', target: 't2'}
touch /tmp/hello_world
```


And if `target` is not specified for a cell in a multi-target notebook, the first target from setup stanza will be used by default:

```bash|{type:'command'}
ls -al /tmp/hello_world
```

Now you can run the two Docable cells above ☝. First execute the cell with **t2** target to create a temp file. Then execute the second cell which uses **t1** target by default to confirm this file does not exist (two separate environments).


You can also use this `target` property in terminal cells. 

    ```bash|{type:'repl', target: 't1', 'background-color': '#00345c'}
    ```

Here is a rendered terminal for **t1** target:

```bash|{type:'repl', target: 't1', 'background-color': '#00345c'}
```

and another one for t2 target:

```bash|{type:'repl', target: 't2', 'background-color': '#013d17'}
```

Feel free to play around with these two terminals to confirm they are connected to different targets.

## Final Thoughts on Workshops

* To receive credit for completing workshops, you will most likely have to submit screenshots or a pdf of the tutorial (`Print > Save As PDF`). Each workshop will have specific instructions on what to turn in.
* The academic integrity policy applies to all workshops. Do not work together unless otherwise specified.
* Remember, any workshop content (including this one) is eligible to be on the exam.

### [Programming Languages ⏭️](Coding.md)