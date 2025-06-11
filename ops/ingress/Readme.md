## using ingress and ingress controller instead of directly using the reverse-proxy like nginx

- we will using the ingress and the ingress-controller instead of directly using the nginx
- ingress uses => ingress-controller for reverse proxy like (nginx ingres-controller) and the loadbalancer service for it.

# steps

- install the nginx ingress-controller
  -- install with manifests
  apply this kubectl apply -f https://raw.githubusercontent.com/nginx/kubernetes-ingress/v5.0.0/deploy/crds.yaml
  this will install the nginx-ingress-controller and the loadbalancer service along with it
- create an ingress.yml file
