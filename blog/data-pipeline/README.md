# data-pipeline

The "data pipeline orchestration at scale" demo from the OrchStep blog post
[Data pipeline orchestration at scale](https://orchstep.dev/blog/data-pipeline-orchestration-at-scale).

```bash
orchstep run etl --var run_date=2026-04-23
orchstep run etl --dry-run    # preview the fan-out + gates, run nothing
```

`extract` fans out three sources in parallel; each dataset is gated by the shared
`quality` module; `finally` always drops the staging tables. Every step is
echo-only, so it runs anywhere.
