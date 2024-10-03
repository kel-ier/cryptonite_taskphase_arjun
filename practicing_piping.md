#Practicing Piping 
    ##Redirecting output 
        echo PWN > COLLEGE
    
    ##Redirecting more output 
        /challenge/run > myflag
    
    ##Appending output 
        /challenge/run >> the-flag   // creates file the-flag with first half of the output 
        echo stdout >> the-flag  // adds second half
    
    ##Redirecting errors 
        /challenge/run >myflag 2> instructions
            // directly stores the output into myflag and any errors(which are instructions here) into instruction

    ##Redirecting input 
        echo COLLEGE > PWN
        /challenge/run < PWN
            //Don't understand where this would be used, need to look into this

    ##Grepping stored results 
        /challenge/run > /tmp/data.txt
        grep pwn.college /tmp/data.txt
    
    ## Grepping live output 
        /challenge/run | grep pwn.college
            //output of /challenge/run (right of |) taken and compared with grep (opn left of|)

    ##Grepping errors 
        /challenge/run 2>&1 | grep pwn.college
            //>& used to send output from one stream to the other. By using 2>&1 we send all the error output into the standard output, which is then taken as input for grep
        
    ##Duplicating piped date with tee
        /challenge/pwn | tee pwnout | /challenge/college
        cat pwnout
        /challenge/pwn --secret 0Qpk0e6R | /challenge/college
    
    ##Writing to multiple programs 
        /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
            //Took some time because I didn't send the output to the file location using >()
    
    ##split-piping
        /challenge/hack 1> >(/challenge/planet) 2> >(/challenge/the)
            /*Tried so many different iterations of this line. tried using multiple processes substitutions and piping variations.
            read through both references to get a better understanding of the way the streams work
            not until much later did it cross my mind that I had to use 1> >(command) rather than 1>(command) because in my mind the syntax was running similar to 2>&1 */
            

        