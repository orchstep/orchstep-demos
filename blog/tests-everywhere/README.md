# tests-everywhere

The demo from the OrchStep blog post
[Run your tests the same way everywhere](https://orchstep.dev/blog/running-tests-the-same-way-everywhere).

```bash
orchstep run test     # unit + integration + lint, then assert they passed
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `go test` / `golangci-lint` commands to make it live. The same `orchstep run
test` is what your CI calls.
