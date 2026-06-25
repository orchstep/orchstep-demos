# sre-runbooks

The demo from "OrchStep for SREs": triage, safe restart, and error-budget runbooks as executable steps.

    orchstep menu                 # pick a task interactively
    orchstep run <task>           # run one task
    orchstep run <task> --dry-run # preview the resolved plan, run nothing

All steps are echo-only and side-effect free, so the workflow runs anywhere.
