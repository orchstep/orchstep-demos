# validate-config-ci

The "validate config in CI before prod" demo from the OrchStep blog post
[Validate config in CI before prod](https://orchstep.dev/blog/validate-config-in-ci-before-prod).

```bash
orchstep lint                          # structure + syntax
orchstep validate deploy --strict      # strict static check of one task
orchstep run check                     # runtime assertions on the config
orchstep run check --var stage=qa      # fails the gate: stage is unknown
```

The three commands form a PR gate: lint catches shape problems, `validate
--strict` catches unresolved references, and `check` asserts the values are
sane. Steps only `echo`, so it is safe to run anywhere.
