# slo-gates

The "SLO and error-budget gates" demo from the OrchStep blog post
[SLO and error-budget gates](https://orchstep.dev/blog/slo-and-error-budget-gates).

```bash
orchstep run gate --var service=checkout
orchstep run gate --var target_pct=100   # raise the bar to see the freeze branch
orchstep run gate --dry-run              # preview the promote/freeze branch, run nothing
```

`availability` emits a literal percentage so the demo runs anywhere. Every step is echo-only.
