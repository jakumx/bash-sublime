aboutme
=======

* Josué
* México
* I like coding, Scout from childhood who enjoys camping, loves video games and Star Wars.
* mx.linkedin.com/in/josvera/


# Open Sublime on terminal(zsh) by custom command

name_file.sh

    #!/bin/bash
    if [ $1 ]
    then
      echo $1
      open -a Sublime\ Text $1
    else
      PWD= pwd
      open -a Sublime\ Text $PWD
    fi

set permission `chmod +x name_file.sh`

add to .zshrc `$ vim ~/.zshrc`
   
    alias sublime="/path/to/file/name_file.sh"
    
on terminal and path to file use `sublime`
