# same-yml-ci

Demo for the OrchStep blog post
[The same orchstep.yml locally and in CI](https://orchstep.dev/blog/the-same-orchstep-yml-locally-and-in-ci).

```bash
orchstep run ci                      # same command you run on the runner
orchstep run ci --var target=production
orchstep run ci --dry-run            # preview the plan, run nothing
```

The steps only `echo`, so it is safe to run anywhere — swap them for your real
lint / test / build commands to make it live. The point: this exact file runs
the same on your laptop and in CI, with plain logs and a real exit code.
