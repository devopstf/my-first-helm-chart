## Simple Helm Demo

This repo contains a quite simple _Helm Chart_ for demo purposes.
It is intended to be used on top of _minikube_ single-node K8s cluster.
The demo is based on [Amy Chen's session in KubeCON 2017](https://www.youtube.com/watch?v=vQX5nokoqrQ), and [Paul's blog post](http://tech.paulcz.net/blog/getting-started-with-helm/).
It's going to be structured as follows:

* Showing helm basic folders structure

```
$ helm create helm
Creating helm
tree helm
helm
+-- charts
+-- Chart.yaml
+-- templates
¦   +-- deployment.yaml
¦   +-- _helpers.tpl
¦   +-- ingress.yaml
¦   +-- NOTES.txt
¦   +-- service.yaml
+-- values.yaml
2 directories, 7 files
```

* Installing our first helm chart based on a simple nginx container deployed with 3 replicas, and a nginx ingress.
* Showing how values can be used within helm charts for customizing our deployments.
* Using plain ``kubectl`` commands for doing the same deployment.
