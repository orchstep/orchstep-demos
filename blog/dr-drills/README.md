# dr-drills

The "rehearse disaster recovery" demo from the OrchStep blog. Back up, restore
to a throwaway target, verify the data is there, and emit a report.

    orchstep run drill            # run the rehearsal
    orchstep run drill --dry-run  # preview the plan, run nothing
