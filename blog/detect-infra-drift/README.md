# detect-infra-drift

The "detect infra drift on a schedule" demo from the OrchStep blog.

    orchstep run check                       # plan -> count diffs -> alert if drift
    orchstep run check --var stack=staging
    orchstep run check --dry-run             # preview the plan, run nothing

The plan step's diff count is stubbed for the demo, so every step is echo-only
and runs anywhere.
