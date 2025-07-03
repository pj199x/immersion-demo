## Deploying the initial version

To deploy the first version of your application:

```
git clone --depth=1 https://github.com/pj199x/immersion-demo.git
helm install helm-voting-app immersion-demo/helm-blue-green
```

## Perform the second deployment

To deploy the updated version using a Blue/Green strategy:

```
helm upgrade helm-voting-app immersion-demo/helm-blue-green --set db.image.tag=17-alpine --set redis.image.tag=7.4.4-alpine
```
