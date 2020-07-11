NAME = mapitman/linux-tools
TAG ?= latest
default: build

build:
	docker build -t $(NAME):$(TAG) .
	docker tag $(NAME):$(TAG) $(NAME):latest

push:
	docker push $(NAME):$(TAG)
	docker push $(NAME):latest

run:
	docker run --rm -it $(NAME):latest
