# docker-cfn-sphere

Wrap cfn-sphere inside a docker container

## Usage

```bash
docker run --rm  --workdir=$(pwd) -v $(pwd):$(pwd) -v $HOME/.aws:/root/.aws cfn-sphere cf <command>
```

In order to make it easier to use, create an alias with this (use single quotes):

```bash
alias cf='docker run --rm  --workdir=$(pwd) -v $(pwd):$(pwd) -v $HOME/.aws:/root/.aws cfn-sphere cf'
```

Now the alias is going to work like the cfn-sphere command.
