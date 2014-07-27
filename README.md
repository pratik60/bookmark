bookmark
========

This is a very handy functionality that lets us bookmark folders, and easily navigate to them in the future, rather than manually creating aliases for navigating into each folder.

Sample Use Case

```bash
cd /webapps/app1
bookmark firstapp
```

then next time  you could directly do
```bash
go app1
```

rather than having to cd into the folder manually. 


List of Commands

a) Bookmark a folder. If no arguments are passed, it will create a bookmark with that current folder's name.

```bash
cd /webapps/app2
bookmark [name]
```

The file where bookmarks are saved (.bookmarks) will look like this
/webapps/app1              firstapp
/webapps/app2              app2

b) Unbookmark functionality has been added as well. Will unbookmark current folder if no name is specified.

```
unbookmark [name]
```

Error message on unbookmarking a folder that doesn't exist. If you were inside a specific folder which has been bookmarked, it would be removed from list of bookmarks.

c) Show Bookmarks to see list of bookmarks

```
bookmarksshow 
```

d) Go - Command to navigate to a folder. Supports completion as well.

```
go app2
```

P.S. - Been using this functionality for a long time, can't remember its original author. Code's been heavily modified with a lot of functionalities added by me now. Credit to him/her as well :-)

