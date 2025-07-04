# [Argo Rollouts](https://argo-rollouts.readthedocs.io/en/stable/)

## Install the Argo Rollouts controller in your cluster
```bash
git clone --depth=1 https://github.com/pj199x/immersion-demo.git
helm dependency update immersion-demo/argo-rollouts
helm template argo-rollouts immersion-demo/argo-rollouts --namespace argo-rollouts --values immersion-demo/argo-rollouts/values.yaml
helm upgrade argo-rollouts immersion-demo/argo-rollouts --install --namespace argo-rollouts --values immersion-demo/argo-rollouts/values.yaml --create-namespace --timeout 10m --wait
```
_Ref: [Argo Rollouts Chart](https://github.com/argoproj/argo-helm/tree/main/charts/argo-rollouts)_
