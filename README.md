# Git practice

This is a repository for git practice for collaboration.

Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

### Undoing Things

One of the common undos takes place when you commit too early and possibly forget to add some files, or you mess up your commit message. If you want to redo that commit, make the additional changes you forgot, stage them, and commit again using the --amend option.

```
$ git commit --amend
```

This command takes your staging area and uses it for the commit. If you're made no changes since your last commit, then your snapshot will look exactly the same, and all you'll change is your commit message.

The same commit-message editor fires up, but it already contains the message of your previous commit. You can edit the message the same as always, but it overwrites your previous commit.

```
$ git commit -m 'Initial commit'
$ git add forgotten_file
$ git commit --amend
```

You end up with a single commit -- the second commit replaces the results of the first.
