# indie-ship

The "OrchStep for indie hackers" demo from the OrchStep blog.

    orchstep run ship      # build -> deploy (retry + rollback) -> smoke
    orchstep run backup    # point a cron at this
    orchstep run digest    # your daily numbers

Steps are `echo`-only, so the whole thing runs anywhere with no side effects.
