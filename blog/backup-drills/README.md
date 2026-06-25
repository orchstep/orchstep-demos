# backup-drills

The backup + restore-drill workflow from the OrchStep blog post
[Backups and restore drills you can trust](https://orchstep.dev/blog/backups-and-restore-drills-you-trust).

```bash
orchstep run backup           # dump, upload (with retry), verify, prune
orchstep run restore-drill    # rehearse a restore and assert it isn't empty
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `pg_dump` / object-store commands to make it live. Failed uploads and restores
fire a `catch:` alert.
