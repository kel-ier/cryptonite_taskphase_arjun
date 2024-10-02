#Comprehending commands
    ##cat
        executed: cat flag

    ##catting absolute paths
        cat /flag

    ##catting practice
        cat /usr/share/fonts/flag
    
    ##grepping for a needle in a haystack 
        grep pwn.college path

    ##listing files 
        cd to /challenge
        ls //to show files
        ./9221.... //to open file
    ##touching files 
        used touch to create required files 
    
    ##removing files 
        used rm to remove delete.me file
    
    ##hidden files 
        opened / directory
        used ls -a to display hidden files 
        used cat to display contents under the flag file
    
    ##epic file system quest
        Literally just followed the clues using cd and ls to find the right file 

    ##making directory
        Created directory using mkdir, created file using touch
    
    ##finding files
        find / -name flag
        used cat on each presented path to see if its a directory or not 
        when not directory, it displayed the flag

    ##linking files 
        cat challenge/catflag
        ln -s /flag  ~/not-the-flag //Took a bit of time, had to remove the pre existing not a flag file
        /challenge/catflag
        //need to look further into hard and soft linking 
