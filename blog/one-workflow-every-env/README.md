# one-workflow-every-env

The inline-environments demo from the OrchStep blog post
[One workflow, every environment](https://orchstep.dev/blog/one-workflow-every-environment).

```bash
orchstep run deploy --env dev          # replicas=2  db=dev-db   log=debug
orchstep run deploy --env staging      # replicas=4  db=staging-db
orchstep run deploy --env production   # replicas=10 db=prod-db  log=error
orchstep run deploy --env production --var replicas=1   # --var still wins
```

The steps only `echo`, so it is safe to run anywhere. The same `deploy` task
serves every environment — `--env` swaps the values, not the workflow.
