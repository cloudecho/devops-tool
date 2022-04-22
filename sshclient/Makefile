MY_IMAGE="cloudecho/sshclient:latest"

build:
	sudo docker build -t ${MY_IMAGE} .

push: build
	#cat ~/.docker/pass | sudo docker login --username=cloudecho --password-stdin
	sudo docker push ${MY_IMAGE}