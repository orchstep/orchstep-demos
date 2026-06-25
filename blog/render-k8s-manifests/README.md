# render-k8s-manifests

The "render Kubernetes manifests per environment" demo from the OrchStep blog post
[Render Kubernetes manifests per environment](https://orchstep.dev/blog/render-kubernetes-manifests-per-environment).

```bash
orchstep run apply --env staging
orchstep run apply --env production       # 5 replicas, prod host
orchstep run apply --env production --dry-run
```

One template, two environments — only the `vars` change. The `apply` step
only `echo`s, so it is safe to run anywhere; swap it for a real `kubectl apply`
to make it live.
