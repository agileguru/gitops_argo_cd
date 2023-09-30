# How to Install ARGO-CD

* kubectl apply -f 1_namespace.yaml
* kubectl apply -f 2_kcert.yml
* kubectl apply -f 3_install.yaml -n argocd
* kubectl apply -f 4_ingress.yaml
* kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d

# Install cli tool to manage argo cd

Please follow the guide [here](https://argo-cd.readthedocs.io/en/stable/cli_installation/) to install the argo cli

# Set your local enviroment 

Execute command after changing devops.demo.agileguru.org for host and argo for path

    $ argocd login devops.demo.agileguru.org --grpc-web-root-path argo

