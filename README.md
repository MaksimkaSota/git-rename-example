# Git file rename issues
Git has no rename file conception. The file can be renamed, but if it differs in content too much it will consider it a new file.  

In this case we lose the content tracking of a file, it may make it harder to study a codebase in the future.  
If these files just come into and out of existence from nowhere, it's a problem for content tracking.  
***
### Branch `delete-add`:
When a file has been renamed and changed in one commit, GitHub displays it as one deleted file and one added file.  
This means that a multiline file will be reviewed without context, which is very useless!  
***
### Branch `rename-modify`:
When a file has been renamed and changed in several commit, GitHub displays it as one renamed file.  
This means that a multiline file will be reviewed with context (in last specific commit), which is very useful!  
