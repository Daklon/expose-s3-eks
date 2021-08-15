# expose-s3-eks

## Description

On this repository resides the eksctl yaml files used to create a cluster on aws eks.
Eksctl will also create the roles, policies and service accounts needed to deploy an external-dns and s3-proxy

## Usage
You must have your aws credentials configured on the machine where you are going to run eksctl

```
$ eksctl create cluster -f eksctl-cluster-definition.yaml
```
## Related Repositories

[s3-proxy Helm Chart](https://github.com/Daklon/s3-exposer-helm)

[Flux root repository](https://github.com/Daklon/flux-s3-exposer)


## Sources:
[pottava aws-s3-proxy](https://github.com/pottava/aws-s3-proxy)

[eksctl iam serviceaccounts usage](https://eksctl.io/usage/iamserviceaccounts/)

[Amazon docs iam roles for service accounts](https://docs.aws.amazon.com/es_es/eks/latest/userguide/iam-roles-for-service-accounts.html)

[Nginx ingress controller configuration](https://kubernetes.github.io/ingress-nginx/user-guide/nginx-configuration/)

[Cert Manager](https://cert-manager.io/docs/tutorials/acme/ingress/)

[External DNS for aws](https://github.com/kubernetes-sigs/external-dns/blob/master/docs/tutorials/aws.md)
