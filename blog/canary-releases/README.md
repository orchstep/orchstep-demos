# canary-releases

The "canary releases, step by step" demo from the OrchStep blog post
[Canary releases, step by step](https://orchstep.dev/blog/canary-releases-step-by-step).

```bash
orchstep run release --var version=2.5.0
orchstep run release --dry-run    # preview the promote/abort branch, run nothing
```

The `watch` step emits a literal `healthy` so the demo runs anywhere. Swap its
`echo` for a real metrics query (and flip the value to see the `abort` branch).
