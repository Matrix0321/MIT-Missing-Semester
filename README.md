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
