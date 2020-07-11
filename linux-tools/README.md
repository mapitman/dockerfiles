# linux-tools

I use this on my Windows system to run commands like telnet, netcat, etc.

## Usage

```sh
docker run --rm -it mapitman/linux-tools { telnet, nc, etc. }
```

I set up some functions in my `.bashrc` to run various tools in the Docker container:

```sh
dig () {
    docker run -it --rm mapitman/linux-tools dig $@
}

host () {
    docker run -it --rm mapitman/linux-tools host $@
}

pwgen () {
    docker run -it --rm  mapitman/linux-tools pwgen "$@"
}

telnet () {
    docker run -it --rm mapitman/linux-tools telnet "$@";
}

nc () {
    docker run -it --rm mapitman/linux-tools nc "$@";
}
```

