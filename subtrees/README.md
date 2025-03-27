The `one` project is cloned from https://github.com/moonrepo/git-subtree-test using this command:

```
git subtree add --prefix subtrees/one https://github.com/moonrepo/git-subtree-test.git master --squash
```

This squashes the entire history into 1 commit, and commits it to the main repo. It does not create a separate checkout like submodules! To pull in new changes, run this command:

```
git subtree pull --prefix subtrees/one https://github.com/moonrepo/git-subtree-test.git master --squash
```

More info: https://www.atlassian.com/git/tutorials/git-subtree
