# coverage-matrix

The validation-matrix demo from the OrchStep blog post
[A coverage matrix that catches missing vars](https://orchstep.dev/blog/a-coverage-matrix-that-catches-missing-vars).

```bash
orchstep validate deploy            # prints the env x var coverage matrix
orchstep validate deploy --strict   # exit non-zero if any referenced var is unsupplied (CI gate)
orchstep validate deploy --json     # machine-readable for CI dashboards
```

`target` is supplied by the concrete `*-dev` / `*-production` files but NOT by the
`nonprod` / `prod` group layers — `validate` shows exactly that before you ship.
