# qa-test-gates

The "OrchStep for QA engineers" demo from the OrchStep blog.

    orchstep run smoke                  # fast pre-merge smoke checks
    orchstep run test --var shards=4    # sharded suite + flaky quarantine
    orchstep run repro --var case=PROJ-481   # one-command bug reproduction

Steps are `echo`-only, so the whole thing runs anywhere with no side effects.
