NAME = mapitman/php-cli
default: build

build:
	docker build --build-arg VCS_REF=`git rev-parse --short HEAD` --build-arg BUILD_DATE=`date -u +"%Y-%m-%dT%H:%M:%SZ"` -t $(NAME):8 .

push:
	docker push $(NAME):8

run:
	docker run -it --rm $(NAME):8
