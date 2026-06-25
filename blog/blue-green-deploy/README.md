# blue-green-deploy

Demo for the OrchStep blog post
[Blue/green deploys with instant rollback](https://orchstep.dev/blog/blue-green-deploys-with-instant-rollback).

```bash
orchstep run deploy --var version=2.5.0
orchstep run deploy --dry-run            # preview the plan, run nothing
```

Deploys to the idle slot, verifies it before any traffic moves, then flips
atomically. A failed flip triggers the `catch` rollback, so the live slot never
serves a bad build. Steps only `echo`, so it runs anywhere — swap them for your
real deploy / health-check / traffic-switch commands.
