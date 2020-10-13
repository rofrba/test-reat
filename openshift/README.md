# Pipelines CI/CD

## Crear desde CLI

### CI

``` bash
oc new-app --template ci-pipeline -p APP_NAME=frontend -p GIT_REPO=ssh://git@10.200.172.71/flow/s2i-frontend.git -p GIT_BRANCH=openshift -n flow-dev
```

### CD

```bash
oc new-app --template cd-pipeline -p APP_NAME=frontend -p GIT_REPO=ssh://git@10.200.172.71/flow/s2i-frontend.git -p GIT_BRANCH=openshift -n flow-dev
```