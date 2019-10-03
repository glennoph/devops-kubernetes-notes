# Install minikube
* goto https://github.com/kubernetes/minikube/releases
* select latest release (v1.4.0)
* Installation - Getting started
* https://github.com/kubernetes/minikube/releases
* download minikube 1.4 deb file
* check that virtulation is allowed
* >`minikube start`

Done! kubectl is now configured to use "minikube"

## incr memory 
> `minikube config set memory 4096`

# install kubectl
## option 1
* goto https://kubernetes.io/docs/tasks/tools/install-kubectl/
## option 2 snap
> `sudo snap install kubectl --classic`
## check version
> `kubectl version`

* version 
`Client Version: version.Info{Major:"1", Minor:"16", ...`

# run hello world
> `kubectl run hello-minikube --image=gcr.io/google_containers/echoserver:1.4 --port=8080`

* deployment.apps/hello-minikube created
> `kubectl expose deployment hello-minikube --type=NodePort`
* expose via node port
> `minikube service hello-minikube --url`
* get url
* goto url can add / and path 
