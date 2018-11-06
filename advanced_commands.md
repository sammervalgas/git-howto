# Advanced Commands #

### Config

```bash

# Add alias for short command

# Locally [Global]
    git config [--global] alias.st status
    git config [--global] alias.rst reset
    git config [--global] alias.co checkout
# Ex
    git st
    git rst
    git co
    git publish
```

#### Instructions
```bash
    git config [--global] alias.publish '!git checkout master && git pull && git checkout dev && git rebase master && git checkout master && git merge dev && git push'

    # --> ! : Allow valid command lines
    # --> git checkout master: change Working Directory to branch master
    # --> git pull: Update branch master atualiza o histórico da branch master
    # --> git checkout develop: change Working Directory to branch develop
    # --> git rebase master: Update  HEAD of branch develop to receive changes of the branch master
    # --> git checkout master: Return to branch master
    # --> git merge develop: Merge branch develop to master
    # --> git push: Send changes to remote repository
```
[Git Config](https://git-scm.com/docs/git-config)


### Merge

Terminologia
|Symbol|Description|
|:-----:|:-----:|
|<<<<|Remote HEAD Changes|
|====|Separation|
|>>>>|Local Changes|

```bash
git merge

git mergetool --tool-help

# Free tools  kdiff3, Meld ou P4Merge
git mergetool -t [nome_do_programa]

```
> Técnica:
>   Para evitar trabalhos com merge é altamente recomendado que sejam realizados commits pequenos (git commit) e sincronização  (git pull) frequentemente.

### Rebase

```bash
# Atualiza uma branch com base em outra
git rebase [branch-from] [branch-to]
git rebase master develop
# --continue deve ser utilizado após a resolução manual de conflitos;
# --skip faz com que suas alterações sejam descartadas;
# --abort volta atrás em todo o processo de rebase

```

# Revert & Reset

```bash
# Revert file that was commit.
    git checkout [file-name]

# Revert --> Undo a specific commit
    git log
    git revert *[-n] [commit-hash]

# reset -->  discard commits
    git reset [commit-hash | HEAD] ] [file-name] [--soft] [--hard]
# reset --> Discard last commit
    git reset --hard HEAD~1

```

# Stash
Store changes to work later

```bash
    # Store untracked files
    git stash

    # List stash
    git stash list

    # restore untracked files again to repo
    git stash pop

    # specifc stash
    git stash apply [stash{0}]

    # Remove stash files
    git stash drop

    # Exclude all stash states
    git stash clear
```

# Search commits right

```bash
git log

git bisect bad HEAD
git bisect good [commit-hash]
git bisect [good] [bad]
```

# Cherry-pick

The cherry-pick command allows a specific commit to be selected and taken to another branch.

```bash
    git cherry-pick [commit-hash]
    # [-n = --no-commit]
    git cherry-pick -n [commit-hash] 
    git help gitrevisions | grep cherry-pick
    git cherry-pick abcd..1234

```

> Note:
> Take care with this approach 'cause can easily cause merge conflicts