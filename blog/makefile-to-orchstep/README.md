# makefile-to-orchstep

The "from Makefile to OrchStep in an afternoon" demo from the OrchStep blog.

    orchstep run build    # deps -> compile
    orchstep run test     # build -> unit
    orchstep run check    # lint + vet, in parallel
    orchstep run clean

Targets become tasks, prerequisites become `task:` steps, and `.PHONY` is the
default. Every step is an `echo`, so it runs anywhere.
