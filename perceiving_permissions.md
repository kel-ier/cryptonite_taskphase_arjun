#Perceiving permissions

    ##Changing File ownership
        chown <new owner> <file name>
    
    ##Groups and Files 
        chgrp <group> <file name>
        //id can be used to find which groups the current user is a part of 
    
    ##Fun with group names 
        Change group of /flag to user's group
    
    ##Changing permissions
        //chmod allows you to tweak permissions with the mode format of WHO+/-WHAT, where WHO is user/group/other and WHAT is read/write/execute.
        chmod guo+rwx /flag 
            // ls -l to check access
        
    
    ##Executable files 
        guo+rwx /challenge/run
    
    ##Permission tweaking practice
        followed given instructions
    
    ##Permissions setting practice
        Followed instructions 
    
    ##The SUID bit 
        chmod u+s <file name> //used to set 
    