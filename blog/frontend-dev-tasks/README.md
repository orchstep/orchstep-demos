# frontend-dev-tasks

The demo from "OrchStep for frontend developers": run the same checks CI runs, then ship a preview build.

    orchstep menu                 # pick a task interactively
    orchstep run <task>           # run one task
    orchstep run <task> --dry-run # preview the resolved plan, run nothing

All steps are echo-only and side-effect free, so the workflow runs anywhere.
