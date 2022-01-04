### Shells

Shell _commands_ can also be edited and run directly in Docable. We will primarily be using Bash shells for this course. In the editor below, type `pwd` and run the command to see the working directory path for this workshop.

<!-- 
targets:
    - type: docker
      name: command-example
      image: node:12-buster
-->
```bash|{type:'command', shell:'bash'}

```
**Variables**
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

Docable also provides several types of terminals, including bash, zsh, and Read, Evaluate, Print, Loop (REPL) terminals for programming languages such as node, python, Ruby (irb), and Java (JShell).

### [Bash Shells ⏭️](Shells.md)