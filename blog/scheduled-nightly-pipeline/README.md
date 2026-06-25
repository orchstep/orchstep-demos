# scheduled-nightly-pipeline

The "scheduled CI jobs and nightly pipelines" demo from the OrchStep blog.

    orchstep run nightly                       # what the nightly cron triggers
    orchstep run nightly --var run_id=weekly
    orchstep run nightly --dry-run             # preview the plan, run nothing

Every step is echo-only, so it runs anywhere.
