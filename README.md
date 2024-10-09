# argocd-helmfile


## Build image

```shell
make build
```

Image name : docker.io/laurentpoirierfr/argocd-helmfile:v0.1.0


```shell
curl https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml -o install-argo-cd.yaml
```

Replace : quay.io/argoproj/argocd:v2.12.3
By      : docker.io/laurentpoirierfr/argocd-helmfile:v0.1.0 


```shell
kubecrl create ns argocd 
kubectl apply -n argocd -f install-argo-cd.yaml
```


## References

* https://www.opsmx.com/blog/argo-cd-installation-into-kubernetes-using-helm-or-manifest/