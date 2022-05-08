# Tennis Racket [489 Points]

I am tasked to connect to a server and use Racket to obtain the flag hidden in the server.

## Solution

1. Connect to Server
```
nc tennis1.nypinfsecctf.tk 8010
```

2. List contents of current directory       
```
(directory-list)
```     
   
* A file called "flag" is found, thought it was a directory at first but navigating to it gives errors so this leads me to believe that it was a file instead of a directory.           

3. List contents of flag file to obtain flag
```
(file->list "flag")
```
