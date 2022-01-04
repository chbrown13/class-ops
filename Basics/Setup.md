# Getting Started

To successfully build software, you need a properly configured environment with a variety of tools. Unfortunately, creating consist work enviroments for a development team can be difficult and frustrating, especially in a classroom environment, due to various operating systems, personal configurations, coding editor preferences and setups, etc. Thus, for the majority of workshops for CS 5704 this semester we will be using Docable to create a consistent development environment for everyone to complete activities. Below is a brief tutorial on how to use this interactive tutorial system.

### Files

Docable allows users to edit and store _files_. Below is a sample text file. You may edit the contents of a file by clicking in the editor below and typing whatever you want. Try updating the `/tmp/docable.txt` file below. To create or update the file in the interactive tutorial environment, click on the pencil and paper icon (📝) on the right side of the editor (_Make sure not to forget this step, otherwise you may face problems later in tutorials!_). You should see a message that says SUCCESS: Created file successfully.

```bash|{type:'file',path:'/tmp/docable.txt'}

```

### Scripts

Similarly, Docable is able to provide simple _scripts_ for you to edit and run blocks of code. To edit, change the content within the text editor. To run, click on the play button icon (▶️) on the right side of the editor. The platform supports scripting in JavaScript, Python, Ruby, and Java. Scripts will be indicated with a '[script:]' and the logo of the script's programming language the left side of the coding editor (i.e. the script below is in JavaScript). Modify the first line of the script below to print out `Hello Docable` on the first line and add a new line to print `Welcome to CS5704!`. Running the script should generate a success message with the output.

```js |{type:'script'}
console.log( "Hello World" );
```

Update the print statement below to print `"Hello Docable` (typo included). When this script is run, you should run into a compilation error due to invalid JavaScript syntax.

```js |{type:'script'}
console.log(  );
```

### Shell

Shell _commands_ can also be edited and run directly in Docable. We will primarily be using Bash shells for this course. In the editor below, type `ls` and run the command to see the list of files for this workshop.

```bash|{type:'command', shell:'bash'}

```


### Terminals

Below is a sample text file. You may edit the contents of a file by clicking in the editor below and typing whatever you want. Try updating the `tmp/docable_file` below. To create the file in the interactive tutorial environment, click on the pencil and paper icon (📝) on the right side of the editor. (_When working with files be sure not to forget this step, otherwise it could cause problems later on in tutorials!_)

