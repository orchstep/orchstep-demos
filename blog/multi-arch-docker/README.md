# multi-arch-docker

The "multi-arch Docker images in one workflow" demo from the OrchStep blog post
[Multi-arch Docker images in one workflow](https://orchstep.dev/blog/multi-arch-docker-images-one-workflow).

```bash
orchstep run build --var version=1.3.0
orchstep run build --dry-run    # see one build/push per platform, run nothing
```

Add or drop a platform in `defaults.platforms` and every step that loops over it
follows. Steps only `echo`, so it is safe to run anywhere.
