# k8s-dev-loop

The fast cluster development loop from the OrchStep blog post
[A fast local Kubernetes loop](https://orchstep.dev/blog/a-fast-local-kubernetes-loop).

```bash
orchstep run loop --var tag=dev
orchstep run loop --dry-run     # preview the resolved plan, run nothing
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `docker`, `kind`, and `kubectl` commands to make it live.
