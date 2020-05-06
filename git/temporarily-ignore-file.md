# Temporarily Ignore File in Git

`.gitignore` is the standard mechanism for ignoring a file change, but it can
be convenient to ignore a file personally without making changes to the tracked
.gitignore file. 

## Example Use Cases
* Ignore a local change to tracked configuration file
* Ignore a single file to easily operate on many other files as a batch (i.e. 
the oft-forbidden `git commit -a`)

## Usage

`git update-index --assume-unchanged <file>`

and later to "unignore":

`git update-index --no-assume-unchanged <file>`