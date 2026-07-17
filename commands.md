we use bash which is represented as $ this is a shell.
shell is a interface between os and user which accepts commands from user and sends it to os kernel.
Bash,sh,csh,ksh,zsh are few types of shell.


The Bash shell features
Scripting: The ability to place commands in a file and then interpret (effectively use Bash to execute the contents of) the file, resulting in all of the commands being executed. This feature also has some programming features, such as conditional statements and the ability to create functions 
Aliases: The ability to create short nicknames for longer commands.
Variables: Used to store information for the Bash shell and for the user. These variables can be used to modify how commands and features work as well as provide vital system information.



The structure of the prompt 
sysadmin@localhost:~$
 where sysadmin is username
 localhost is system name
 ~ is current directory 
 $ is bash shell


 NOW WE ENTER INTO ACTUAL COMMANDS
 ls-- it stands for list.when u tpe ls,it lists all the folders(directories)
 Some commands require additional input to run correctly. This additional input comes in two forms: options and arguments.Options are used to modify the core behavior of a command while arguments are used to provide additional information

 LINUX IS CASE SENSITIVE
 ls:
  /etc/ppp directory is used as an argument.
  ---sysadmin@localhost:~$ ls /etc/ppp    The command ls /etc/ppp is used to list the contents of the /etc/ppp directory.
    
    ls -l :it an argument.This is the "long listing" format. Instead of just showing the names of your files, it displays a detailed breakdown of your files.
    ls -r :By default, the ls command alphabetizes your files and folders (from A to Z). Adding the -r flag tells the system to flip that order and list them in reverse alphabetical order (from Z to A).
    ls -lr :it is the combination of above two
    The order of the combined options isn't important. The output of all of these examples would be the same:
        ls -l -r
        ls -rl
        ls -lr
    
    ls -h:The -h flag stands for "human-readable."It makes file sizes easy for humans to read (like 10M or 2G) instead of showing them as giant, confusing numbers of bytes (like 10485760).

    Pressing the Up Arrow ↑ key displays the previous command on the prompt line.
    When the desired command is located, the Left Arrow ← and Right Arrow → keys can position the cursor for editing. Other useful keys for editing include the Home, End, Backspace and Delete keys.
    date command is used to see the date.
    history command is used to see what commands we used earlier.
    If the desired command is in the list that the history command generates, it can be executed by typing an exclamation point ! character and then the number next to the command
    To execute the nth command from the bottom of the history list, type !-n and hit Enter
    To execute the most recent command type !! and hit Enter


    echo command is used to dislay the output in the terminal.

    COMMAND TYPES:
          The type command can be used to determine information about command type.
          There are several different sources of commands within the shell of your CLI including internal commands, external commands, aliases, and functions.

      INTERNAL COMMANDS:
            these are also called as built_in commands which are built in shell itself.
            ex:cd (change directory) command as it is part of the Bash shell. When a user types the cd command, the Bash shell is already executing 
               sysadmin@localhost:~$ type cd                                     
               cd is a shell builtin
               The type command identifies the cd command as an internal command
                
        EXTERNAL COMMANDS:
            External commands are programs (binary executable files) stored on your computer.
             "which" command Shows where an external command is stored.
                   sysadmin@localhost:~$ which ls                                       
                   /bin/ls                                                               
                   sysadmin@localhost:~$ which cal                                        
                   /usr/bin/cal
             "type" command tells u the what type of command it is:
                sysadmin@localhost:~$ type cal                                      
                cal is /usr/bin/cal

                sysadmin@localhost:~$ type echo                                     
                echo is a shell builtin
                sysadmin@localhost:~$ which echo                                        
                /bin/echo

                Using the -a option of the type command displays all locations that contain the command named:

                      sysadmin@localhost:~$ type -a echo                                      
                      echo is a shell builtin                                                
                      echo is /bin/echo


                      





     

    

