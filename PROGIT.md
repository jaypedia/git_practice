# Pro git

### git cherry-pick

The git cherry-pick command is used to take the change introduced in a single Git commit and try to re-introduce it as a new commit on the branch you're currently on.

### Tagging

Like most VCSs, Git has the ability to tag specific points in a repository's history as being important. Typically, people use this functionality to mark release points.

##### Listing your tags

Listing the existing tags in Git is straightforward.

```
$ git tag
v1.0
v2.0
```

##### Creating tags

Git supports two types of tags : lightweight and annotated.

- A lightweight tag is very much like a branch that doesn't change -- it's just a pointer to a specific commit.

- Annotated tags, however, are stored as full objects in the Git database. They're checksummed; contain the tagger name, email, and date; have a tagging message; and can be signed and verified with GNU Privacy Guard (GPG). It's generally recommended that you create annotated tags so you can have all this information; but if you want a temporary tag or for some reason don't want to keep the other information, lightweight tags are available too.
