# Trabalhando com branchs

## Versão 1
---

```
$ git init relatorio
$ cd relatorio
$ code README.md
$ git add README.md
$ git commit -m 'primeira versão do relatório'
```

![](img/v1-4-git-commit-tree-refs.png)
![](img/v1-4-git-commit-refs.png)

```
$ git log --oneline
d12305b (HEAD -> master) adicionando o capítulo 1
```

## Versão 2
---

```
$ code README.md
$ code capitulos/capitulo-1.md
$ git add README.md capitulos/capitulo-1.md
$ git commit -m 'adicionando o capítulo 1'
```

![](img/v2-3-git-commit-tree-refs.png)
![](img/v2-3-git-commit-refs.png)

```
$ git log --oneline
d12305b (HEAD -> master) adicionando o capítulo 1
5bf530e primeira versão do relatório
```

## Criando a branch `cap-2`
---

```
$ git checkout -b cap-2
Switched to a new branch 'cap-2'
```

![](img/b1-git-branch-cap-2-tree-refs.png)
![](img/b1-git-branch-cap-2-refs.png)

```
$ git log --oneline --graph --decorate
* d12305b (HEAD -> master, cap-2)adicionando o capítulo 1
* 5bf530e primeira versão do relatório
```

## Versão 3
---

```
$ code README.md
$ code capitulos/capitulo-2.md
$ git add README.md capitulos/capitulo-2.md
$ git commit -m 'adicionando o capítulo 2'
```

![](img/v3-3-git-commit-tree-refs.png)
![](img/v3-3-git-commit-refs.png)

## Merge do `cap-2` para o `master`
---

```
$ git checkout master
```

![](img/b2-git-branch-master-tree.png)

```
$ git merge cap-2
```

![](img/m1-git-merge-tree-refs.png)

## Resumindo
---

### Versão 1

![](img/v1-4-git-commit-tree-snapshot.png)<br>

### Versão 2

![](img/v2-3-git-commit-tree-snapshot.png)

### Criando a branch `cap-2`

![](img/b1-git-branch-cap-2-tree-snapshot.png)

### Versão 3

![](img/v3-3-git-commit-tree-snapshot.png)

### Merge do `cap-2` para o `master`

![](img/b2-git-branch-master-tree-snapshot.png)
![](img/m1-git-merge-tree-snapshot.png)