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

* version Client Version: version.Info{Major:"1", Minor:"16", ...
