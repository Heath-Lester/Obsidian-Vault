<iframe width="100%" src="https://www.youtube-nocookie.com/embed/I4EWvMFj37g?si=wXbsl5oT3htOaFkm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 4px; aspect-ratio: 16/9;"></iframe>

BASH is a command language interpreter called Bourne Again Shell. This language is for interacting directly with the computer through command line.

- It is called shell because it surrounds the operating system kernel as an interface
- Commands are sent through a terminal, to the shell, and is executed by the operating system
- Command `which $SHELL` will return the file location of the shell
- BASH is also a programming language that allows users to write scripts
- The bash profile file will allow you to change the look and behavior of the shell
- Shell scripts use the `.sh` file extension or no file extension
- First line in shell script files should be a shebang `#!` followed by the path to BASH `/usr/bin/bash`
- Variables are set with all capitalized names and accessed with `$`
```bash
#!/usr/bin/bash
echo 'my first bash script ✨'

GREET="Howdy Partner"
echo $GREET
```
- To execute BASH or Shell files simply type the name or file path in the terminal
- BASH can use do while loops and if statements
- You can run multiple processes in parallel by using the `&` sign
- To give a file executable permissions, use the `chmod` command with the `u+x` or `x` flags and the file
- The `u` flag limits the permissions to the active user