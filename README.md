# split_preserve_history

Little demo to keep Git history when splitting a file (blame).

Principle :
* we want to split file A content
* create a branch, rename A to C and change code as needed
* on the original branch, move A to B and change code as needed
* merge branches, resolve conflict
* you get files B and C all of which contains A history !


Found this procedure in this excellent article : [Splitting files while preserving history in git — musicmatzes blog](https://beyermatthias.de/splitting-files-while-preserving-history-in-git).  

Other resources on the same subject : 

* Same procedure done with the octopus merge strategy, no conflicts to handle (!!) : [How do I split a file into two while preserving git line history? - The Old New Thing](https://devblogs.microsoft.com/oldnewthing/20190916-00/?p=102892)
* Still same procedure, explained in a Stack Overflow thread, and some answers point out some difficulties with it (but lacks of details imho...) : [Git copy file preserving history - Stack Overflow](https://stackoverflow.com/questions/16937359/git-copy-file-preserving-history/44036771#44036771)
* Stack Overflow thread explaining why we can see a code moved from one file to another : [version control - How does git track source code moved between files? - Stack Overflow](https://stackoverflow.com/questions/1728922/how-does-git-track-source-code-moved-between-files)

See also a tool to automate the process :
https://github.com/potherca-bash/git-split-file
