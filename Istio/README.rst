

Mini-kube
=========

::

  brew cask reinstall minikube

::

  minikube start --memory=8192 --cpus=4 --kubernetes-version=v1.10.1

::

  kubectl config use-context minikube

::

  curl -L https://git.io/getLatestIstio | sh -

  cd istio-1.0.5

  export PATH=$PWD/bin:$PATH


After https://istio.io/docs/setup/kubernetes/quick-start/ :

::

   kubectl apply -f install/kubernetes/helm/istio/templates/crds.yaml

::

  kubectl apply -f install/kubernetes/istio-demo.yaml

::

  export MINIKUBE_IP=$(minikube ip)
  

AKS
===

https://docs.microsoft.com/en-us/azure/aks/istio-install
