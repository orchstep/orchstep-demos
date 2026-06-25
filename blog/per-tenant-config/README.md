# per-tenant-config

The per-tenant loop demo from the OrchStep blog post
[Per-tenant config at scale](https://orchstep.dev/blog/per-tenant-config-at-scale).

```bash
orchstep run provision           # loops every tenant, each with its own region + tier
orchstep run one --var id=acme   # provision a single tenant on demand
```

The roster lives in `defaults.tenants` — adding a customer is a one-line edit, not a
new task. Each iteration sets a per-tenant `env:` for the tool it calls. The steps
only `echo`, so it runs anywhere.
