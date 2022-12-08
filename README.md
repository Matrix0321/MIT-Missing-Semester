# MIT-Missing-Semester
Some exercises after lectures.
## Lecture 1
### 1.Create a new directory called missing under /tmp.
```mkdir /tmp/missing```
### 2.Look up the touch program. The man program is your friend.
```man touch```
### 3.Use touch to create a new file called semester in missing.
```touch /tmp/missing/semester```
### 4.Write the following into that file, one line at a time:
> #!/bin/sh  
> curl --head --silent https://missing.csail.mit.edu  

Answer:  
```echo '#!/bin/bash' > semester```  
```echo "curl --head --silent https://missing.csail.mit.edu" >> semester```  
### 5.Try to execute the file, i.e. type the path to the script (./semester) into your shell and press enter. Understand why it doesn’t work by consulting the output of ls (hint: look at the permission bits of the file).
```./semester```  
```ls -l```  
The permission string is -rw-r--r--, so I am not allowed to execute this file.  
### 6.Run the command by explicitly starting the sh interpreter, and giving it the file semester as the first argument, i.e. sh semester. Why does this work, while ./semester didn’t?
We don't have permission to run ```semester```, but we can still run ```sh```.
### 7.Look up the chmod program (e.g. use man chmod).
The answer is clear.
