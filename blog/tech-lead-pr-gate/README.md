# tech-lead-pr-gate

The "OrchStep for tech leads" demo from the OrchStep blog.

    orchstep run gate --var branch=feature/new-api   # the merge gate as code

`lint` and `unit` are reusable tasks the `gate` task calls. Steps are
`echo`-only, so the whole thing runs anywhere with no side effects.
