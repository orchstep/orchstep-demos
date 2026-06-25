# devops-pipelines

The demo from "OrchStep for DevOps engineers": one ci task your laptop and your pipeline both run.

    orchstep menu                 # pick a task interactively
    orchstep run <task>           # run one task
    orchstep run <task> --dry-run # preview the resolved plan, run nothing

All steps are echo-only and side-effect free, so the workflow runs anywhere.
