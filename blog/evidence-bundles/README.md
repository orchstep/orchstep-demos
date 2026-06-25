# evidence-bundles

The "evidence bundle for compliance" demo from the OrchStep blog. Gather the
artifacts an auditor asks for, hash them, and seal them into one bundle.

    orchstep run bundle                       # bundle the default release
    orchstep run bundle --var release=2026.6.0
    orchstep run bundle --dry-run             # preview the plan, run nothing
