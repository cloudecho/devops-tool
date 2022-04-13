MY_IMAGE="cloudecho/maven-ex:3.8.5-jdk-11"

build:
	sudo docker build -t ${MY_IMAGE} .

push: build
	#cat ~/.docker/pass | sudo docker login --username=cloudecho --password-stdin
	sudo docker push ${MY_IMAGE}