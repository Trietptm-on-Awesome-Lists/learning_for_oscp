# Manipulating Files
this lesson will introduce you to the following commands:
- **cp** - copy files and directories
- **mv** - move or rename files and directories
- **rm** - remove files and directories
- **mkdir** - create directories

## Wildcards
Special characters to help you rapidly specify groups of filenames is called wildcards.
wildcards allow you to select filenames based on patterns of characters. The table below list the wildcards and what they select:
|**Wildcard**|**Meaning**|
|:--|:--|
|*|Matches any characters|
|?|Matches any single characters|
|[character]|Mathces any character that is a member of the set characters. you can use POSIX character class instead.
	[:alnum:]	Alphanumeric characters
	[:alpha:]	Alphabetic characters
	[:digit:]	Numerals
	[:upper:]	Uppercase
	[:lower:]	Lowercase
|[!characters]|Matches any character that is not a member of the set characters|
|:--|:--|

## cp
The **cp** program copies files and directories. 
```bash
[me@linuxbox me]$ cp file1 file2
```
```bash
[me@linuxbox me]$ cp file... directory
```
if you specified i option and the file you want to make exists, the user is prompted
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg0ODc4NDE2Nl19
-->