# argocd-sync-test-sample
+ This is the sample code for verifying Pre/PostSync in ArgoCD.
  + https://argoproj.github.io/argo-cd/user-guide/resource_hooks/

# Prerequisites
+ You need to create an `imagePullSecrets` for login to Dockerhub etc. with the name `regcred` beforehand referring to the following.
  + https://kubernetes.io/docs/tasks/configure-pod-container/pull-image-private-registry/

+ Also, for kubeconfig for Kuberenetes cluster to be deployed, you need to create `secret` in advance as follows.

```
kubectl create secret generic secret-kubeconfig --from-file=/[YOUR_KUBECONFIG_PATH]/.kube/config 
```
