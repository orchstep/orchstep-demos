# promote-build

The "promote one build through every environment" demo from the OrchStep blog post
[Promote one build through every environment](https://orchstep.dev/blog/promote-one-build-through-every-environment).

```bash
orchstep run deploy --env dev
orchstep run deploy --env staging
orchstep run deploy --env production   # manual-approval branch
orchstep run deploy --env staging --dry-run
```

The same `{{ vars.artifact }}:{{ vars.version }}` flows through all three
environments — only the target and policy change. Steps only `echo`, so it is
safe to run anywhere.
