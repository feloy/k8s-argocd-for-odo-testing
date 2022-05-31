Create an application on the cluster you want to configure for odo testing:

```shell
$ argocd app create odo-testing \
    --repo https://github.com/feloy/k8s-argocd-for-odo-testing.git \
    --path . \
    --directory-recurse \
    --dest-server https://kubernetes.default.svc \
    --dest-namespace default
```
