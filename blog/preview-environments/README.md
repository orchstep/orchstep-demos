# preview-environments

The "ephemeral preview environments per PR" demo from the OrchStep blog post
[Ephemeral preview environments per PR](https://orchstep.dev/blog/ephemeral-preview-environments-per-pr).

```bash
orchstep run up   --var pr=482       # on PR open / push
orchstep run down --var pr=482       # on PR close
orchstep run up   --var pr=482 --dry-run
```

The PR number is the only input — the namespace, deploy target, and URL all
derive from it. Steps only `echo`, so it is safe to run anywhere.
