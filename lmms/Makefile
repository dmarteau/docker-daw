SHELL:=bash

NAME=lmms
VERSION:=1.2

BUILDIMAGE=$(NAME):$(VERSION)

all: build

build:
	docker build --rm $(BUILD_ARGS) -t $(BUILDIMAGE) \
		-t $(NAME):latest --cache-from=$(NAME):latest $(DOCKERFILE) .

clean-all:
	docker rmi -f $(shell docker images $(BUILDIMAGE) -q)

clean:
	docker rmi $(BUILDIMAGE)

