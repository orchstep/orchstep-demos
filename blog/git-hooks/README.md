# git-hooks

The demo from the OrchStep blog post
[Git hooks that don't fight you](https://orchstep.dev/blog/git-hooks-that-dont-fight-you).

```bash
orchstep run precommit   # fast: format + lint (call from .git/hooks/pre-commit)
orchstep run prepush     # heavier: format + lint + test (call from pre-push)
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `gofmt` / `golangci-lint` / `go test` commands to make it live.
