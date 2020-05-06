# Temporarily Ignore File in Git

`.gitignore` is the standard mechanism for ignoring a file change, but it can
be convenient to ignore a file personally without making changes to the tracked
.gitignore file. 


## Usage

`git update-index --assume-unchanged <file>`

and later to "unignore":

`git update-index --no-assume-unchanged <file>`

## Notes
Files can still be explicity added, by name or as a side-effect of `git commit -a`.

## Source
[Nick Quaranto: Git Ready - temporarily ignoring files](http://gitready.com/intermediate/2009/02/18/temporarily-ignoring-files.html)