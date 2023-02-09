# Modify-PS1-Path

# Introduction

In Linux, the command prompt, often known as the shell or BASH, is where you do the majority of your work (Bourne-Again Shell). Your commands are translated by the shell before being sent to the operating system for execution.
Have you considered modifying the shell prompt?

This guide will show how to modify or personalise your Linux BASH prompt.

## Prerequisites :

* A system running Linux
* Access to a command line/terminal
* A user account with sudo or root privileges

#### Default BASH Prompt

The default BASH prompt is the one you see when you first open a terminal or command line. It usually looks something like this :

![ps1](https://user-images.githubusercontent.com/124764401/217745471-715a0f96-54bd-4041-b558-17dd5f5bfd10.png)

#### Modified BASH Prompt

![ps1modified](https://user-images.githubusercontent.com/124764401/217745522-54f422d3-1398-4bcf-9a79-2d70822120f8.png)


------------------------
## Change Bash Prompt in Linux Permanently

Open the BASH configuration file for editing:
Follow this step:

```
sudo -i
vim /etc/bashrc
```

We have to change the PS1 path.
Initial PS1 Path will look like this : PS1="[\u@\h \W]\\$ " 
Change it to

```
PS1="\n\[\e[01;33m\]\u\[\e[0m\]\[\e[00;37m\]@\[\e[0m\]\[\e[01;36m\]\h\[\e[0m\]\[\e[00;37m\] \t \[\e[0m\]\[\e[01;35m\]\w\[\e[0m\]\[\e[01;37m\] \[\e[0m\]\n$ "
```

You can type bash to execute changes OR Exit the terminal and open again to execute changes

#### External Source
Use the below link to customise your own shell prompt.

```
https://bashrcgenerator.com/
```

