# dotenv-done-right

The dotenv load-order demo from the OrchStep blog post
[dotenv done right](https://orchstep.dev/blog/dotenv-done-right).

```bash
orchstep run show   # common.env baseline, app.env overrides AWS_REGION, overrides.env? skipped
```

What it shows:

- **Load order** — `app.env` overrides `AWS_REGION` from `common.env` because it loads later.
- **Optional `?`** — `overrides.env?` is absent here; the trailing `?` makes that a skip, not an error.
- **`<required>`** — `DATABASE_URL` must arrive from a dotenv file (or CI); a run without it fails fast.
- **`env:` precedence** — the `scoped` step sets `LOG_LEVEL=trace`, which wins for that step only.

The steps only `echo`, so it runs anywhere.
