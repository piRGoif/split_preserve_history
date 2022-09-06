# split_preserve_history

Little demo to keep Git history when splitting a file (blame).

Principle :
* we want to split file A content
* create a branch, rename A to C and change code as needed
* on the original branch, move A to B and change code as needed
* merge branches, resolve conflict
* you get files B and C all of which contains A history !


Found this procedure in this excellent article : [Splitting files while preserving history in git — musicmatzes blog](https://beyermatthias.de/splitting-files-while-preserving-history-in-git).  
Same procedure done with the octopus merge strategy, with no conflicts : [How do I split a file into two while preserving git line history? - The Old New Thing](https://devblogs.microsoft.com/oldnewthing/20190916-00/?p=102892)

See also a tool to automate the process :
https://github.com/potherca-bash/git-split-file
