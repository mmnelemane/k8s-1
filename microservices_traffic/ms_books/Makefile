buildimage:
	docker build . -t books_t

testlocalimage: buildimage
	docker run -d -p 3000:3000 books_t

build-minikube-image:
	eval $(minikube docker-env)
	docker build . -t books_t
