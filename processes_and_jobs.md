#Processes and Jobs
   
    ##Listing processes 
        ps aux || ps -ef

    ##Killing processes 
        kill -pid
    
    ##Interrupting processes 
        ctrl c
    
    ##suspending process
        ctrl z
    
    ##Resuming process 
        fg //resume process
    
    ##Backgrounding process
        bg //resume process in background
    
    ##Foregrounding process 
        fg can be used to bring forth a program from the background 

    ##Starting background process
        '&' can be used to directly start a process in the background

    ##Process exit codes 
        processes that succeed give a 0 as exit code and those that fail give non zero values 
        echo $?  //? is used to access the exit code 
    

    