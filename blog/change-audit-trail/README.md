# change-audit-trail

The "every change leaves a trail" demo from the OrchStep blog. Policy checks
and approval gate the change; a hashed, chained record makes it tamper-evident.

    orchstep run apply                                  # default low-risk change
    orchstep run apply --var change=CHG-1099 --var risk=high
    orchstep run apply --dry-run                        # preview the plan, run nothing
