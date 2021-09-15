# kustomize-argocd-sealedsecrets-sample

Repositório de uma POC (prova de conceito): Subir um Redmine + Postgres no Kubernetes, utilizando:

* **Kustomize** para organizar código/configuração de implantação da aplicação;
* **Sealed-Secrets** para gerenciar as credenciais;
* **ArgoCD** para sincronizar/monitorar a implantação da aplicação.

# Kubernetes

Versão: v1.21.2

```
kubectl create ns sealed-secrets
```

 # Sealed Secrets

* Versão v0.16.0: https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.16.0/controller.yaml
* Alterado o namespace de `kube-system` para `sealed-secrets`
* Alterado a apiVersion do RBAC para: `rbac.authorization.k8s.io/v1`

