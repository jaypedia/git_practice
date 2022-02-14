# Git Commit message convention

##### Feb 14, 2022

---

```
<type>(<scope>): <subject>
```

## 1. 'type' must be one of the following mentioned below

- build: Build related changes (eg: npm related/ adding external dependencies)
- chore: A code change that external user won't see (eg: change to .gitignore file or .prettierrc file)
- feat: A new feature
- fix: A bug fix
- docs: Documentation related changes
- refactor: A code that neither fix bug nor adds a feature
  - (eg: You can use this when there is **semantic changes** like renaming a variable/ function name)
- perf: A code that improves performance
- style: A code that is related to styling
  - formatting, missing semi colons, etc; no production code change
- test: Adding new test or making changes to existing test

## 2. 'scope' is optional

- Scope must be noun and it represents the section of the section of the section of the codebase

## 3. 'subject'

- use imperative, present tense (eg: use "add" instead of "added" or "adds")
- don't use dot(.) at end
- don't capitalize first letter

---

### Reference

[Dev | Git commit message convention that you can follow!](https://dev.to/i5han3/git-commit-message-convention-that-you-can-follow-1709)

[Karma | Git Commit Msg](http://karma-runner.github.io/1.0/dev/git-commit-msg.html)
