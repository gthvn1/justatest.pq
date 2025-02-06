# Intro

- This is the repo to keep track of guilt patchqueue of [justatest](https://github.com/gthvn1/justatest)
- Currently it is based on v0.2

# Setup

- clone the upstream justatest
```sh
$ git clone https://github.com/gthvn1/justatest.git
$ cd justatest
```

- Then clone the patchset in `.git/patches`
```sh
$ git clone https://github.com/gthvn1/justatest.pq.git
```

- Create the status file. We don't keep this file because we want to start with clean status.
```sh
$ touch .git/patches/patchqueue/status
```

- Switch to the patchqueue branch and you are ready to apply the patches by doing:
```sh
$ git switch -c patchqueue v0.2
$ guilt push -a
```
