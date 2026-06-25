# feature-flags-config

The "feature flags from config" demo from the OrchStep blog post
[Feature flags from config](https://orchstep.dev/blog/feature-flags-from-config).

```bash
orchstep run flags                          # flags as configured in defaults
orchstep run flags --var new_checkout=true  # flip one flag for this run
orchstep run flags --var beta_search=true --var stage=production
orchstep run flags --dry-run                # see which gates fire, run nothing
```

Flags are plain `vars`, so a `--var` flip or an `--env` selection changes
behavior without touching code. Steps only `echo`, so it is safe to run anywhere.
