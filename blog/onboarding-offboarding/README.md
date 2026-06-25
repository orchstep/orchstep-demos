# onboarding-offboarding

The "onboarding and offboarding automation" demo from the OrchStep blog post
[Onboarding and offboarding automation](https://orchstep.dev/blog/onboarding-and-offboarding-automation).

```bash
orchstep run onboard --var person=jordan
orchstep run offboard --var person=jordan
orchstep run onboard --dry-run    # preview the plan, run nothing
```

Every step is phrased to be idempotent ("ensure ..."), so rerunning is a no-op.
All steps are echo-only, so it runs anywhere.
