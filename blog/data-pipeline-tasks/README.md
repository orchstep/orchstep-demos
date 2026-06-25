# data-pipeline-tasks

The demo from "OrchStep for data engineers": an ETL task with retries and quarantine, plus a partition backfill loop.

    orchstep menu                 # pick a task interactively
    orchstep run <task>           # run one task
    orchstep run <task> --dry-run # preview the resolved plan, run nothing

All steps are echo-only and side-effect free, so the workflow runs anywhere.
