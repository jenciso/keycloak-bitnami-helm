# KEYCLOAK via helmfile

We are using helmfile to provision the keycloak from bitnami/keycloak helm repository

## Values

Get the complete values with comments:
```shell
helm inspect values oci://registry-1.docker.io/bitnamicharts/keycloak > values.yaml
helm show values oci://registry-1.docker.io/bitnamicharts/keycloak > values.yaml
```

Get a simplified values list via helmfile:
```shell
helmfile write-values --output-file-template values.yaml
```
