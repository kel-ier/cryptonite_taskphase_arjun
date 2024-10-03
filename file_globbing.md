#File Globbing 
    ##Matching with *
        cd /ch*  //to open directory
    
    ##Mathching with ? 
        cd /?ha??enge //? used to check for anything i with only that number of letters, substituting ? for any character
    ##Matching with []
        cd /challenge/files
        /challenge/run file_[bash]
    
    ##Matching paths with []
        /challenge/run /challenge/files/file_[bash] //[] used to check for given letters in that position 
        //using the path as an argument 
    
    ##Mixing globs
        moved to /challenge/files 
         /challenge/run [cep]*
         //Each file started with a diff letter 
    
    ##Exclusionary Globbing 
        /challenge/run [!pwn]* //!used to exclude any files starting with given arguments
    
