# Git Multiple Remote

This repository stores some references links to using Git with multiple remote repositories.

## Additional Remote

```bash
# git remote add REMOTE-ID REMOTE-URL
git remote add gh git@github.com:brucechanjianle/git-multiple-remote
```

## Remove Remote
```bash
# git remote remove REMOTE-ID
git remote remove gh
```

## List Remotes
```bash
git remote -v
```

## Push to Multiple Remotes
```bash
git remote add all git@github.com:brucechanjianle/git-multiple-remote
# Re-register remote as a push URL
git remote set-url --add --push all git@github.com:brucechanjianle/git-multiple-remote
# Add a push URL to a remote
git remote set-url --add --push all git@gitlab.com:brucechanjianle/git-multiple-remote.git
```

And now you can push :D
```bash
# git push all BRANCH
git push all master
```

## References

- https://jigarius.com/blog/multiple-git-remote-repositories
