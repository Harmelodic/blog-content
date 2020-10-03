When using something like `kd` within GitLab's CI/CD, you'll need a K8s Service Account and thus a token for that K8s Service Account to allow the deployment agents access to cluster.

```sh
kubectl create serviceaccount gitlab-sa
```

This will create a service account but we'll need to grant it permission to perform things like deployments.

```sh
kubectl create rolebinding gitlab-edit --clusterrole=edit --serviceaccount=default:gitlab
```

Then you'll need to get the token:

```sh
kubectl get secrets
```

```sh
kubectl get secret <SECRET_NAME> -o json | jq -r .data.token | base64 -D
```

---

K8s Rolebinding Permissions for Service Accounts: https://kubernetes.io/docs/reference/access-authn-authz/rbac/#service-account-permissions

K8s User facing Cluster Roles: https://kubernetes.io/docs/reference/access-authn-authz/rbac/#user-facing-roles
