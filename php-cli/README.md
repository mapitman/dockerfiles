# php-cli

This is a slightly modified version of the offical php-cli-alpine
Docker image. I have added _git_ and _zip_ so I can use this to build
composer packages.

## Usage

I use this to work on php without having to install it on my system.  

Example usage:

```sh
docker run -it --net=host -v /${PWD}:/workdir -w //workdir mapitman/php-cli
```

I use `--net=host` to make it easier to connect to my 
[mitmproxy container](https://hub.docker.com/r/mitmproxy/mitmproxy/).
