# Gitflow cheatsheet

[https://nvie.com/posts/a-successful-git-branching-model/](https://nvie.com/posts/a-successful-git-branching-model/)

[http://danielkummer.github.io/git-flow-cheatsheet/index.pt_BR.html](http://danielkummer.github.io/git-flow-cheatsheet/index.pt_BR.html)

## Commands

```bash

git init

git flow init

# feature
# cria uma branch de feature a partir da develop
git flow feature start feature-001
# mescla a branch feature na develop
# deleta a branch feature
# retorna para a branch develop
git flow feature finish feature-001
# push da branch feature
git flow feature publish feature-001
# pull da branch feature
git flow feature pull feature-001

# release
git flow release start release-001
git flow release finish release-001
git flow release publish release-001
git flow release pull release-001

# hotfix
git flow hotfix start hotfix-001
git flow hotfix finish hotfix-001
git flow hotfix publish hotfix-001
git flow hotfix pull hotfix-001

```
