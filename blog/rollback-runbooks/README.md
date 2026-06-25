# rollback-runbooks

The "rollback runbooks you can rehearse" demo from the OrchStep blog post
[Rollback runbooks you can rehearse](https://orchstep.dev/blog/rollback-runbooks-you-can-rehearse).

```bash
orchstep run rollback --var to=2.3.0 --dry-run   # rehearse, run nothing
orchstep run rollback --var to=2.3.0             # execute for real
```

`catch:` handles a failed revert, `finally:` always notifies. Steps only `echo`,
so the rehearsal — and the real thing — is safe to run anywhere.
