# local-task-runner

The "retire your deploy.sh" demo from the OrchStep blog post
[Replace the bash script you keep rewriting](https://orchstep.dev/blog/replace-the-bash-script-you-keep-rewriting).

```bash
orchstep menu                 # pick a task interactively
orchstep run build            # run one task
orchstep run deploy --var version=2.4.0 --env production
orchstep run deploy --dry-run # preview the resolved plan, run nothing
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `docker` / `kubectl` commands to make it live.
