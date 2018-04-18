git-status-interactive
======================

Produce an editable list of file statuses, so you can decide whether to add/ignore/remove/... each file. One of the 2,067,087 projects on Github about Git (as of this writing).

The procedure for using this script:

* Type `git istatus`.

* Your favorite editor opens. There, you see the output from `git status`, which is mostly
a list of files that need to be somehow handled.

* You edit the file to specify what happens to every file. At the top is a list of 
instructions for some basic operations: put an `a` at the head of a line to add a
file, an `i` to ignore it from now on, an `ea` to edit then add (which you'll do if
you're merging), an `r` to remove the file from the repository, and so on.

* When you exit your editor, your instructions are run.    


The full writeup is at this blog: http://modelingwithdata.org/arch/00000031.htm .


## Installation
        
To allow the `git istatus` command above, try this command from your bash prompt, from any git repository:

```git config --add alias.istatus \!/your/path/to/git-status-interactive```

Or if you have the permissions to make global changes to the git config:

```git config --global --add alias.istatus \!/your/path/to/git-status-interactive```
