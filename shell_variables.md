#Shell Variables 
    ##Printing Variables 
        echo $FLAG
    
    ##Setting Variables 
       PWN=COLLEGE
        // $ used only while accessing the values inside variable, called variable expansion
    
    ##Multi Word Variables
        PWN="COLLEGE YEAH"
            //Strings work similar 
    
    ##Exporting Variables 
        export is used to make the variables accessible to any further child shell of the main shell 
            //similar to inheritance 
    
    ##Printing Exported Variables 
        env | grep pwn.college
            env prints the values in every exported variable in the given shell 
    
    ##Storing Command Output 
        PWN=$(/challenge/run)
        //$used here for command substitution

    ##Reading Input 
        read PWN
            //-p is the argument used to give prompt for input

    ##Reading Files 
        read PWN < /challenge/read_me
        
