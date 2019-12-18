  bash_navigator is a tool to jump quickly in your bash navigation history
  
  
![preview_image](https://user-images.githubusercontent.com/9435855/40840582-97f2b53c-65a7-11e8-95e7-99af9668dc42.png)

~~~
NAME  
       bash_navigator is a tool to jump quickly in your bash navigation history  
       IMPORTANT! Each shell instance has its own navigation history by default.

ARGUMENTS  
        -s (--single-nav-hist) : share the same navigation history beetween all your shell instances 

SYNOPSIS  
        bb [delta]
        bbb  
        bf [delta]  
        bff  
        bj [jump_index]  
        bh  
        bhelp  

AVAILABILITY  

       bash, zsh

DESCRIPTION  
       IMPORTANT! Each shell instance has its own navigation history by default.
        
        bb          bash back, move back 
        bbb         bash first, move back to first path 
        bf          bash forward, move forward 
        bff         bash last, move forward to last path 
        bj          bash jump, move specific index path 
        bh          bash history, show navigation paths history and indexes
        bhelp       bash help, show help 

EXAMPLES  
        bhelp       show bash navigator help page
        bh          show navigation history
        bj          navigation history jump dialog (needs dialog)
        bj 78       go to the 78th path in navigation history
        bb          go back in navigation history 
        bb 4        go back 4 times in navigation history
        bbb         go to first path in navigation history
        bf          go forward in navigation history
        bf 6        go forward 6 times in navigation history
        bff         go to last path in navigation history
       
NOTES  
  
   Installation:  
       Put something like this in your $HOME/.bashrc or $HOME/.zshrc:

              source /path/to/bash_navigator.sh  

       If you prefer to share the same navigation history beetween all your shell instances: 

              source /path/to/bash_navigator.sh -s  

       Restart your shell (zsh/bash), cd around to build up the db.
       To verify if the db is building up run the bash navigator history command:

              bh

        NOW ENJOY, MOVE FASTER!!!

   Configuration:  
              IMPORTANT! These  settings  should  go  in  .bashrc/.zshrc BEFORE the above source command.

              Set $_BASH_NAV_HIST_DB_FOLDER         change the navigation database folder (default ~/.cache/bash_navigator).
              Set $_BASH_NAV_HIST_DB_MAX_SIZE       change the number of paths to save in the navigation history (default 100).
              Set $_BASH_NAVIGATOR_BACK             change bash back command (default bb) 
              Set $_BASH_NAVIGATOR_FORWARD          change bash forward command (default bf) 
              Set $_BASH_NAVIGATOR_SHOW_HISTORY     change bash history command (default bh) 
              Set $_BASH_NAVIGATOR_FORWARD          change bash forward command (default bf) 
              Set $_BASH_NAVIGATOR_JUMP             change bash jump command (default bj) 
              Set $_BASH_NAVIGATOR_FORWARD          change bash forward command (default bf) 
              Set $_BASH_NAVIGATOR_JUMP_TO_FIRST    change bash jump to first command (default bbb) 
              Set $_BASH_NAVIGATOR_JUMP_TO_LAST     change bash jump to last command (default bff) 

      Configuration example:  
              _BASH_NAV_HIST_DB_FOLDER="~/.cache/bash_navigator"
              _BASH_NAV_HIST_DB_MAX_SIZE=20
              source /path/to/bash_navigator.sh -s
  
PROJECT  
      https://github.com/abdoulayeYATERA/bash_navigator
~~~
