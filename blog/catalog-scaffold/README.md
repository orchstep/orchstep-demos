# catalog-scaffold

The "scaffold + register + smoke test" demo from the OrchStep blog. One task
takes a service from nothing to a cataloged, health-checked entry.

    orchstep run new                         # scaffold the default service
    orchstep run new --var service=billing   # name the new service
    orchstep run new --dry-run               # preview the plan, run nothing
