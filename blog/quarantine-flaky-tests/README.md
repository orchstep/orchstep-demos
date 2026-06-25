# quarantine-flaky-tests

The "quarantine flaky tests automatically" demo from the OrchStep blog.

    orchstep run test               # retry flaky tests, record any that still fail
    orchstep run test --dry-run     # preview the plan, run nothing

Every step is echo-only, so it runs anywhere.
