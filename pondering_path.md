#Pondering Path 
    
    ##The PATH variable 
        Removed the value of path so the /challenge/run could not access rm 
    
    ##Setting PATH 
     PATH=/challenge/more_commands/
        //this removes bare name access to all other typical commands 
    
    ##Adding Commands 
        mkdir scripts
        nano ~/scripts/win  //cat /flag in win 
        cd scripts
        chmod guo+x
        cd ..
        /challenge/run

    ##Hijacking commands 
        ls <dir> | grep rm //used the directories in PATH to find the rm command
        nano ~/scripts/rm  ///usr/bin/cat /flag  in rm
        PATH=~/scripts
        /challenge/run
        
