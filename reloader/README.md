# [Reloader](https://docs.stakater.com/reloader/index.html)

## Install Reloader in your cluster
```bash
git clone --depth=1 https://github.com/pj199x/immersion-demo.git
helm dependency update immersion-demo/reloader
helm template reloader immersion-demo/reloader --namespace reloader --values immersion-demo/reloader/values.yaml
helm upgrade reloader immersion-demo/reloader --install --namespace reloader --values immersion-demo/reloader/values.yaml --create-namespace --timeout 10m --wait
```
_Ref: [Reloader Upstream Chart](https://github.com/stakater/Reloader/tree/master/deployments/kubernetes/chart/reloader)_
