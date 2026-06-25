# credential-rotation

The "rotate secrets on a schedule" demo from the OrchStep blog post
[Rotate secrets on a schedule](https://orchstep.dev/blog/rotate-secrets-on-a-schedule).

```bash
orchstep run rotate --output json      # what cron/systemd calls
orchstep run rotate --dry-run          # preview the rotation, change nothing
```

The task mints a new version, activates it (with retry), asserts it exists,
then writes a structured `AUDIT` line. Steps only `echo`, so it is safe to run
anywhere; wire the resolver and your store in to make it live.
