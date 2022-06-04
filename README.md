# git refusing to merge unrelated histories on git push

`The fatal: refusing to merge unrelated histories` Git error occurs when two unrelated projects are merged (i.e., projects that are not aware of each other’s existence and have mismatching commit histories).

```bash
$ git pull origin main --allow-unrelated-histories

# Or master
# Or just try with origin

$ git pull origin main --allow-unrelated-histories

$ git add .
# Or file name

$ git commit -m "commited"
$ git push

```

`--allow-unrelated-histories` [GIT HUB DOCS](https://git-scm.com/docs/git-merge#Documentation/git-merge.txt---allow-unrelated-histories)

By default, git merge command refuses to merge histories that do not share a common ancestor. This option can be used to override this safety when merging histories of two projects that started their lives independently. As that is a very rare occasion, no configuration variable to enable this by default exists and will not be added.

### On Stack Overflow

[https://stackoverflow.com/questions/37937984/git-refusing-to-merge-unrelated-histories-on-rebase](https://stackoverflow.com/questions/37937984/git-refusing-to-merge-unrelated-histories-on-rebase)
