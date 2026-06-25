# scheduled-jobs

The cron/timer-friendly maintenance task from the OrchStep blog post
[Scheduled jobs without cron soup](https://orchstep.dev/blog/scheduled-jobs-without-cron-soup).

```bash
orchstep run nightly                 # human-readable
orchstep run nightly --output json   # machine-readable for the timer log
```

The exit code is non-zero if any step fails, so cron or a systemd timer records a
real failure. The steps only `echo`, so it is safe to run anywhere.
