VARIABLES--
    A variable is a feature that allows the user or the shell to store data. This data can be used to provide critical system information or to change the behavior of how the Bash shell work. Variables are given names and stored temporarily in memory. There are two types of variables used in the Bash shell: local and environment:
   
       Local variables:
             Local varaiable or shell variables exists only in the current shell which doesnt affect other applications.
             if the variable is already exists then modify the varaible if it doesnt shell creates the variable by default.
             Ex:sysadmin@localhost:~$ variable1='Something'

       Environment variables:
            Environmental variables or global variable are most commonly used variables which are available system-wise in all the shells used by Bash when interpreting and performing tasks.The system automatically recreates environment variables when a new shell is opened. Examples include the PATH, HOME, and HISTSIZE variables. The HISTSIZE variable defines how many previous commands to store in the history list.
            env command is used to display environmental variables.the output is very loong for enviromental variables.
            so we search for specific word or variable.
           
            The export command converts a local variable into an environment variable.

            export variable=value creates and exports a variable in one step.
            The value of a variable can be changed using the assignment (=) operator.
            The unset command removes a variable.
            The $ tells the shell:
                "Use the value stored inside this variable."


        Path Variables:
            One of the most important Bash shell variables to understand is the PATH variable. It contains a list that defines which directories the shell looks in to find commands. If a valid command is entered and the shell returns a "command not found" error, it is because the Bash shell was unable to locate a command by that name in any of the directories included in the path.
            ex:
                sysadmin@localhost:~$ echo $PATH                                        
                /home/sysadmin/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games
                sysadmin@localhost:~$
                The shell checks the directories in the order that they are listed.

         Each of these directories is represented by a path. A path is a list of directories separated by the / character.
         If the command is not found in any directory listed in the PATH variable, then the shell returns an error




    

