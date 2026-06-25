# support-diagnostics

The "OrchStep for support engineers" demo from the OrchStep blog.

    orchstep run diagnose --var account=acme   # collect a diagnostics bundle
    orchstep run escalate --var account=acme   # diagnose + hand off to eng

Steps are `echo`-only, so the whole thing runs anywhere with no side effects.
