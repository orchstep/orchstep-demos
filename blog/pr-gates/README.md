# pr-gates

Demo for the OrchStep blog post
[PR gates that actually gate](https://orchstep.dev/blog/pr-gates-that-actually-gate).

```bash
orchstep run gate
orchstep run gate --var changed_coverage=71   # fails the assert (below floor)
orchstep validate gate --strict               # every var must resolve
```

The gate asserts coverage stays above the floor and validates that every
referenced var resolves before any test runs. Steps only `echo`, so it runs
anywhere — swap them for your real lint / test commands.
