# incident-runbooks

The "runbook as code" demo from the OrchStep blog. Classify severity, fan out
diagnostics in parallel, route by severity, and write an incident record.

    orchstep run respond                # default SEV2 path
    orchstep run respond --var sev=1    # SEV1 paging path
    orchstep run respond --dry-run      # preview the plan, run nothing
