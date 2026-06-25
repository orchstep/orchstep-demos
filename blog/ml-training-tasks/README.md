# ml-training-tasks

The demo from "OrchStep for ML engineers": a train task gated on accuracy, plus a hyperparameter sweep.

    orchstep menu                 # pick a task interactively
    orchstep run <task>           # run one task
    orchstep run <task> --dry-run # preview the resolved plan, run nothing

All steps are echo-only and side-effect free, so the workflow runs anywhere.
