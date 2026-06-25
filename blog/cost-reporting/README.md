# cost-reporting

The "cost reporting automation" demo from the OrchStep blog post
[Cost reporting automation](https://orchstep.dev/blog/cost-reporting-automation).

```bash
orchstep run report --var report_date=2026-04-28
orchstep run report --var budget_usd=3000   # tighten the budget to see the gate fail
orchstep run report --dry-run               # preview the plan, run nothing
```

Pull -> transform -> render -> gate. Every step is echo-only, so it runs anywhere.
