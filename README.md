# helm-example
Source: https://medium.com/containerum/how-to-make-and-share-your-own-helm-package-50ae40f6c221

curl https://purnendu15.github.io/helm-example/index.yaml
helm repo add helm-example https://purnendu15.github.io/helm-example/
helm install helm-example/kubevirt --name=kubevirt --namespace=kube-system

kubectl apply -f vm.yaml -n kube-system
kubectl get vms -n kube-system

kubectl describe vm testvm -n kube-system

