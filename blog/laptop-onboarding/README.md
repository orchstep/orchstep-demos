# laptop-onboarding

The one-command laptop setup from the OrchStep blog post
[One-command onboarding for new laptops](https://orchstep.dev/blog/one-command-onboarding-for-new-laptops).

```bash
orchstep run setup
orchstep run setup --var installed=true   # the idempotent re-run path
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `brew` / `mise` / dotfile commands to make it live.
