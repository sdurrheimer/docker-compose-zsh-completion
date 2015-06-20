# docker-compose-zsh-completion

__UPDATES__ : Zsh completion has been merged in the docker-compose official repository. I will try to keep this repo updated with the official one.

A zsh completion for [docker-compose](https://github.com/docker/compose)

## How to Install

Put this `_docker-compose` into your `~/.zsh/completion` directory, then reload your shell :
```sh
mkdir -p ~/.zsh/completion
curl -L https://raw.githubusercontent.com/sdurrheimer/docker-compose-zsh-completion/master/_docker-compose > ~/.zsh/completion/_docker-compose
exec $SHELL -l
```

At this point, if completion doesn't work, add this to your `~/.zshrc` file, then reload one more time your shell :
```sh
fpath=(~/.zsh/completion $fpath)
autoload -Uz compinit && compinit -i
```
```sh
exec $SHELL -l
```

## Contributors

* [sdurrheimer](http://github.com/sdurrheimer)
