# Jellyfin kustomize

Project that hold an example to deploy jellyfin via k8s kustomize.

## Example Usage

`
kubectl apply -k <./example>
`

### PV
The PV are so configured that it uses an local storage on the k8s server.

### Ingress

In the example we use the k8s NGINX-ingress. Zou need to change it to traffik or an other  that your k8s-ingress-controller will use. 

If you want to upload pictures withe an bigger size you need to adjust

`
  annotations:
    nginx.ingress.kubernetes.io/proxy-body-size: 5m
`






