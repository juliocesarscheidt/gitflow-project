# Gitflow cheatsheet

[https://nvie.com/posts/a-successful-git-branching-model/](https://nvie.com/posts/a-successful-git-branching-model/)

[http://danielkummer.github.io/git-flow-cheatsheet/index.pt_BR.html](http://danielkummer.github.io/git-flow-cheatsheet/index.pt_BR.html)

> init

```bash
git init

git remote add origin https://github.com/juliocesarscheidt/gitflow-project.git

git flow init
```

> feature

```bash
# cria uma branch de feature a partir da develop
git flow feature start feature-001

# mescla a branch feature na develop
# deleta a branch de feature
# retorna para a branch develop
git flow feature finish feature-001

# push da branch feature
git flow feature publish feature-001

# pull da branch feature
git flow feature pull feature-001
```

> release

```bash
# cria uma branch de release a partir da develop
git flow release start release-001

# push da branch release
git flow release publish release-001

# mescla a branch release na master
# add uma tag na versão
# mescla a branch da versão de volta na develop
# deleta a branch de release
git flow release finish release-001

# pull da branch release
git flow release pull release-001
```

> hotfix

```bash
# cria uma branch de hotfix a partir da master
git flow hotfix start hotfix-001

# push da branch hotfix
git flow hotfix publish hotfix-001

# mescla a branch release na master
# add uma tag na versão
# mescla a branch da versão de volta na develop
# deleta a branch de hotfix
git flow hotfix finish hotfix-001

# pull da branch hotfix
git flow hotfix pull hotfix-001

```
