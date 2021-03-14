VERSION=1.0-3.6.2
PROJECT_ID=kubernetes-zookeeper
PROJECT=terencedeng

all: build

build:
	docker build --pull -t ${PROJECT}/${PROJECT_ID}:${VERSION} .

push: build
	gcloud docker -- push ${PROJECT}/${PROJECT_ID}:${VERSION}

.PHONY: all build push
