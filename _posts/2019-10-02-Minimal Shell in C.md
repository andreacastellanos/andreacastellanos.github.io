---
layout: default
title: Minimal Shell in C
type: project
permalink: projects/minimal-shell-in-c
---

NAME
  
    msh – a minimal shell handling up to one pipe and input and output redirection

SYNOPSIS

    msh.c, parser.c, parser.h, Makefile

DESCRIPTION
  
    msh is a minimal shell program, it will work with one pipe, or two commands, 
     and works with input and output redirection.

RUNNING
   
    Makefile is included. Running it is as simple as compiling, by typing “make”. Then to
     run the program, “make run”.

QUITTING
    
    CTRL+C will not work to quit the program, CTRL+\ will successfully make you quit msh.

NOTES
    
    Input/Output redirection does not work with multiple commands, or ones that include pipes. 
    In order to run something like “ls –l | wc > output”, 
        first run: “ls –l > newout”, then run: “wc newout > output”. 
    That will successfully do wc on the ls –l output into the file output.
  
    If you want to run a test script, commented out items starting with the pound sign will not be ran. 
    The pound sign needs to be at the beginning for msh to ignore it.
  
    If you want to run a test script, simply call ./msh <location/to/test/script>
  
    Any program that is viable with execvp, or a standard shell, will work with msh. 


Makefile

![parser.h](/assets/images/projects/minimal shell in c/makefile.png)


main.c

![main.c](/assets/images/projects/minimal shell in c/main.png)


paser.h

![parser.h](/assets/images/projects/minimal shell in c/parser-h.png)


parser.c

![parser.c](/assets/images/projects/minimal shell in c/parser-c.png)


msh.c

![msh.c](/assets/images/projects/minimal shell in c/msh.png)


[back](./)