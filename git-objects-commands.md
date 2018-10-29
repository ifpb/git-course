## Git Objects

## Versão 1
---

```
$ tree -a
.
└── .git
    ├── FETCH_HEAD
    ├── HEAD
    ├── branches
    ├── config
    ├── description
    ├── hooks
    │   ├── applypatch-msg.sample
    │   ├── commit-msg.sample
    │   ├── fsmonitor-watchman.sample
    │   ├── post-update.sample
    │   ├── pre-applypatch.sample
    │   ├── pre-commit.sample
    │   ├── pre-push.sample
    │   ├── pre-rebase.sample
    │   ├── pre-receive.sample
    │   ├── prepare-commit-msg.sample
    │   └── update.sample
    ├── info
    │   └── exclude
    ├── objects
    │   ├── info
    │   └── pack
    └── refs
        ├── heads
        └── tags

10 directories, 16 files
```

```
$ tree -a
.
├── .git
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── info
│   │   └── exclude
│   ├── objects
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       └── tags
└── README.md

10 directories, 17 files
```

```
$ tree -a
.
├── .git
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── objects
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       └── tags
└── README.md

11 directories, 19 files
```

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           └── master
│   ├── objects
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   └── master
│       └── tags
└── README.md

16 directories, 25 files
```

```
$ find .git/objects -type f
.git/objects/89/d7691fbe5e9ffe9647b3392a91187df114e64c
.git/objects/5b/f530e9db9d8489f1822bdd41f04302095dfd03
.git/objects/7a/a496585358593fd6f5ded8e17f8c05202b2661
```

```
$ git cat-file -p 5bf5
tree 7aa496585358593fd6f5ded8e17f8c05202b2661
author Luiz Carlos Rodrigues Chaves <lucachaves@gmail.com> 1540697879 -0300
committer Luiz Carlos Rodrigues Chaves <lucachaves@gmail.com> 1540697879 -0300

primeira versão do relatório
```

```
$ git cat-file -p 7aa4
100644 blob 89d7691fbe5e9ffe9647b3392a91187df114e64c    README.md
```

```
$ git cat-file -p 89d7
# Relatório
```

## Versão 2
---

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           └── master
│   ├── objects
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    └── capitulo-1.md

17 directories, 26 files
```

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           └── master
│   ├── objects
│   │   ├── 1e
│   │   │   └── d94cb8973788c6db7f030d5d70b262e34721cd
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 70
│   │   │   └── 656d380f3e52f0fa96546ac5f202945e539d3a
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    └── capitulo-1.md

19 directories, 28 files
```

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           └── master
│   ├── objects
│   │   ├── 1e
│   │   │   └── d94cb8973788c6db7f030d5d70b262e34721cd
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 70
│   │   │   └── 656d380f3e52f0fa96546ac5f202945e539d3a
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── b2
│   │   │   └── 1b02bfe8db0f16349adc0c87ce3836ed1188be
│   │   ├── c0
│   │   │   └── 104672317ce3bfc5f085f2f01e0bccf8df8c19
│   │   ├── d1
│   │   │   └── 2305b51ecabcb7af0c009778d76e0f5fc7cb8b
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    └── capitulo-1.md

22 directories, 31 files
```

```
$ find .git/objects -type f
.git/objects/b2/1b02bfe8db0f16349adc0c87ce3836ed1188be
.git/objects/d1/2305b51ecabcb7af0c009778d76e0f5fc7cb8b
.git/objects/c0/104672317ce3bfc5f085f2f01e0bccf8df8c19
.git/objects/89/d7691fbe5e9ffe9647b3392a91187df114e64c
.git/objects/5b/f530e9db9d8489f1822bdd41f04302095dfd03
.git/objects/70/656d380f3e52f0fa96546ac5f202945e539d3a
.git/objects/1e/d94cb8973788c6db7f030d5d70b262e34721cd
.git/objects/7a/a496585358593fd6f5ded8e17f8c05202b2661
```

```
$ git cat-file -p b21b
100644 blob 70656d380f3e52f0fa96546ac5f202945e539d3a    capitulo-1.md
```

```
$ git cat-file -p d123
tree c0104672317ce3bfc5f085f2f01e0bccf8df8c19
parent 5bf530e9db9d8489f1822bdd41f04302095dfd03
author Luiz Carlos Rodrigues Chaves <lucachaves@gmail.com> 1540703525 -0300
committer Luiz Carlos Rodrigues Chaves <lucachaves@gmail.com> 1540703525 -0300

adicionando o capítulo 1
```

```
$ git cat-file -p c010
100644 blob 1ed94cb8973788c6db7f030d5d70b262e34721cd    README.md
040000 tree b21b02bfe8db0f16349adc0c87ce3836ed1188be    capitulos
```

```
$ git cat-file -p 7065
# Capítulo 1
```

```
$ git cat-file -p 1ed9
# Relatório

* [Capítulo 1](capitulos/capitulo-1.md)
```

## Criando a branch `cap-2`
---

```
$ git checkout -b cap-2
Switched to a new branch 'cap-2'
```

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           ├── cap-2
│   │           └── master
│   ├── objects
│   │   ├── 1e
│   │   │   └── d94cb8973788c6db7f030d5d70b262e34721cd
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 70
│   │   │   └── 656d380f3e52f0fa96546ac5f202945e539d3a
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── b2
│   │   │   └── 1b02bfe8db0f16349adc0c87ce3836ed1188be
│   │   ├── c0
│   │   │   └── 104672317ce3bfc5f085f2f01e0bccf8df8c19
│   │   ├── d1
│   │   │   └── 2305b51ecabcb7af0c009778d76e0f5fc7cb8b
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   ├── cap-2
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    └── capitulo-1.md

22 directories, 33 files
```

## Versão 3
---

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           ├── cap-2
│   │           └── master
│   ├── objects
│   │   ├── 1e
│   │   │   └── d94cb8973788c6db7f030d5d70b262e34721cd
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 70
│   │   │   └── 656d380f3e52f0fa96546ac5f202945e539d3a
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── b2
│   │   │   └── 1b02bfe8db0f16349adc0c87ce3836ed1188be
│   │   ├── c0
│   │   │   └── 104672317ce3bfc5f085f2f01e0bccf8df8c19
│   │   ├── d1
│   │   │   └── 2305b51ecabcb7af0c009778d76e0f5fc7cb8b
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   ├── cap-2
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    ├── capitulo-1.md
    └── capitulo-2.md

22 directories, 34 files
```

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           ├── cap-2
│   │           └── master
│   ├── objects
│   │   ├── 04
│   │   │   └── 99b9875e95059f55cdc1500e161405adc7b663
│   │   ├── 1e
│   │   │   └── d94cb8973788c6db7f030d5d70b262e34721cd
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 70
│   │   │   └── 656d380f3e52f0fa96546ac5f202945e539d3a
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── a1
│   │   │   └── 32237a8ccc03260cbbb8a5a3c2f31d5ec38109
│   │   ├── b2
│   │   │   └── 1b02bfe8db0f16349adc0c87ce3836ed1188be
│   │   ├── c0
│   │   │   └── 104672317ce3bfc5f085f2f01e0bccf8df8c19
│   │   ├── d1
│   │   │   └── 2305b51ecabcb7af0c009778d76e0f5fc7cb8b
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   ├── cap-2
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    ├── capitulo-1.md
    └── capitulo-2.md

24 directories, 36 files
```

```
$ git cat-file -p 0499
# Capítulo 2
```

```
$ git cat-file -p a132
# Relatório

* [Capítulo 1](capitulos/capitulo-1.md)
* [Capítulo 2](capitulos/capitulo-2.md)
```

```
$ tree -a
.
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── branches
│   ├── config
│   ├── description
│   ├── hooks
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   └── update.sample
│   ├── index
│   ├── info
│   │   └── exclude
│   ├── logs
│   │   ├── HEAD
│   │   └── refs
│   │       └── heads
│   │           ├── cap-2
│   │           └── master
│   ├── objects
│   │   ├── 04
│   │   │   └── 99b9875e95059f55cdc1500e161405adc7b663
│   │   ├── 1e
│   │   │   └── d94cb8973788c6db7f030d5d70b262e34721cd
│   │   ├── 5b
│   │   │   └── f530e9db9d8489f1822bdd41f04302095dfd03
│   │   ├── 70
│   │   │   └── 656d380f3e52f0fa96546ac5f202945e539d3a
│   │   ├── 7a
│   │   │   └── a496585358593fd6f5ded8e17f8c05202b2661
│   │   ├── 7f
│   │   │   └── 8fb2fdef15db9d2b60d941b8c0fa3b2661947a
│   │   ├── 89
│   │   │   └── d7691fbe5e9ffe9647b3392a91187df114e64c
│   │   ├── a1
│   │   │   └── 32237a8ccc03260cbbb8a5a3c2f31d5ec38109
│   │   ├── b2
│   │   │   └── 1b02bfe8db0f16349adc0c87ce3836ed1188be
│   │   ├── be
│   │   │   └── b15334f100d7ea785b89f4101ebf8444fb0d6c
│   │   ├── c0
│   │   │   └── 104672317ce3bfc5f085f2f01e0bccf8df8c19
│   │   ├── c6
│   │   │   └── 70a06683623ec87011b39615edba9b0a9d9862
│   │   ├── d1
│   │   │   └── 2305b51ecabcb7af0c009778d76e0f5fc7cb8b
│   │   ├── info
│   │   └── pack
│   └── refs
│       ├── heads
│       │   ├── cap-2
│       │   └── master
│       └── tags
├── README.md
└── capitulos
    ├── capitulo-1.md
    └── capitulo-2.md

27 directories, 39 files
```

```
$ find .git/objects -type f
.git/objects/04/99b9875e95059f55cdc1500e161405adc7b663
.git/objects/b2/1b02bfe8db0f16349adc0c87ce3836ed1188be
.git/objects/be/b15334f100d7ea785b89f4101ebf8444fb0d6c
.git/objects/d1/2305b51ecabcb7af0c009778d76e0f5fc7cb8b
.git/objects/c0/104672317ce3bfc5f085f2f01e0bccf8df8c19
.git/objects/c6/70a06683623ec87011b39615edba9b0a9d9862
.git/objects/89/d7691fbe5e9ffe9647b3392a91187df114e64c
.git/objects/5b/f530e9db9d8489f1822bdd41f04302095dfd03
.git/objects/a1/32237a8ccc03260cbbb8a5a3c2f31d5ec38109
.git/objects/70/656d380f3e52f0fa96546ac5f202945e539d3a
.git/objects/1e/d94cb8973788c6db7f030d5d70b262e34721cd
.git/objects/7f/8fb2fdef15db9d2b60d941b8c0fa3b2661947a
.git/objects/7a/a496585358593fd6f5ded8e17f8c05202b2661
```

```
$ git cat-file -p beb1
100644 blob a132237a8ccc03260cbbb8a5a3c2f31d5ec38109    README.md
040000 tree 7f8fb2fdef15db9d2b60d941b8c0fa3b2661947a    capitulos
```

```
$ git cat-file -p c670
tree beb15334f100d7ea785b89f4101ebf8444fb0d6c
parent d12305b51ecabcb7af0c009778d76e0f5fc7cb8b
author Luiz Carlos Rodrigues Chaves <lucachaves@gmail.com> 1540711122 -0300
committer Luiz Carlos Rodrigues Chaves <lucachaves@gmail.com> 1540711122 -0300

adicionando o capítulo 2
```

```
$ git cat-file -p 7f8f
100644 blob 70656d380f3e52f0fa96546ac5f202945e539d3a    capitulo-1.md
100644 blob 0499b9875e95059f55cdc1500e161405adc7b663    capitulo-2.md
```

## Refs
---

```
$ find .git/refs
.git/refs
.git/refs/heads
.git/refs/heads/cap-2
.git/refs/heads/master
.git/refs/tags
```

## Packfiles
---

```
$ git cat-file -p master^{tree}
100644 blob a132237a8ccc03260cbbb8a5a3c2f31d5ec38109    README.md
040000 tree 7f8fb2fdef15db9d2b60d941b8c0fa3b2661947a    capitulos
```

```
$ git gc
Counting objects: 13, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (13/13), done.
Total 13 (delta 1), reused 0 (delta 0)
```

```
$ git verify-pack -v .git/objects/pack/pack-d4febbb06bee7b93410128e74c121f034758346c.idx
c670a06683623ec87011b39615edba9b0a9d9862 commit 276 184 12
d12305b51ecabcb7af0c009778d76e0f5fc7cb8b commit 276 184 196
5bf530e9db9d8489f1822bdd41f04302095dfd03 commit 233 158 380
a132237a8ccc03260cbbb8a5a3c2f31d5ec38109 blob   95 64 538
70656d380f3e52f0fa96546ac5f202945e539d3a blob   13 22 602
0499b9875e95059f55cdc1500e161405adc7b663 blob   13 22 624
beb15334f100d7ea785b89f4101ebf8444fb0d6c tree   73 84 646
7f8fb2fdef15db9d2b60d941b8c0fa3b2661947a tree   82 79 730
c0104672317ce3bfc5f085f2f01e0bccf8df8c19 tree   73 83 809
1ed94cb8973788c6db7f030d5d70b262e34721cd blob   4 15 892 1 a132237a8ccc03260cbbb8a5a3c2f31d5ec38109
b21b02bfe8db0f16349adc0c87ce3836ed1188be tree   41 52 907
7aa496585358593fd6f5ded8e17f8c05202b2661 tree   37 48 959
89d7691fbe5e9ffe9647b3392a91187df114e64c blob   12 21 1007
non delta: 12 objects
chain length = 1: 1 object
.git/objects/pack/pack-d4febbb06bee7b93410128e74c121f034758346c.pack: ok
```
