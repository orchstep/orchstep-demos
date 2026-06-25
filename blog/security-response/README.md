# security-response

The "security response automation" demo from the OrchStep blog post
[Security response automation](https://orchstep.dev/blog/security-response-automation).

```bash
orchstep run respond --var image=ghcr.io/acme/api:2.0.0
orchstep run respond --var threshold=critical   # raise the bar to see the log-only branch
orchstep run respond --dry-run                  # preview the triage branch, run nothing
```

`scan` emits a literal severity so the demo runs anywhere. Every step is echo-only.
