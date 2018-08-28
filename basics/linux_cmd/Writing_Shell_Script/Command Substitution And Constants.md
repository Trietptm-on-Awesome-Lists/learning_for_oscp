# Command Substitution and Constants
Now, we will add a timestamp to the page to indicate when it was last updated.
add`<p>Updated on $(date +"%x %r %Z") by $USER</p>` below the h1 tag.

The characters "$()" tell the shell, "substitute the results of the enclosed command." 
The *date* command has many features and formatting options. To look at them all, try this:
```bash
[me@linuxbox me]$ date --help | less
```

## Assigning A Command's Result To A Variable
You can also assign the results of a command to a variable:
```bash
right_now=$(date +"%x %r %Z")
```
You can even nest the variables (place one inside another), like this:
```bash
right_now=$(date +"%x %r %Z")
time_stamp="Updated on $right_now by $USER"

## Constants

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkzMDIxMzE1MCwtNDEwMDM0NTExXX0=
-->