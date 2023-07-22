# How to Install ARGO-CD

* kubectl apply -f 1_namespace.yaml
* kubectl apply -f 2_kcert.yml
* kubectl apply -f 3_install.yaml -n argocd
* kubectl apply -f 4_ingress.yaml
* kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d

