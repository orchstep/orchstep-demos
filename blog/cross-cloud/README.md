# cross-cloud

The "cross-cloud orchestration" demo from the OrchStep blog post
[Cross-cloud orchestration](https://orchstep.dev/blog/cross-cloud-orchestration).

```bash
orchstep run provision --var stage=production
orchstep run provision --dry-run    # preview the AWS + GCP fan-out, run nothing
```

`clouds` provisions AWS and GCP in parallel; `verify` checks both in one step.
Every step is echo-only, so it runs anywhere.
