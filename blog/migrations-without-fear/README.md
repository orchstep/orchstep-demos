# migrations-without-fear

The demo from the OrchStep blog post
[Database migrations without the 2am dread](https://orchstep.dev/blog/database-migrations-without-fear).

```bash
orchstep run migrate --var target=production --dry-run   # preview, run nothing
orchstep run migrate --var target=production             # backup + apply + verify
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `pg_dump` / migration-tool commands to make it live.
