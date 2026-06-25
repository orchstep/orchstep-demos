# machine-bootstrap

The "bootstrap a dev machine in one command" demo from the OrchStep blog post
[Bootstrap a dev machine in one command](https://orchstep.dev/blog/bootstrap-a-dev-machine-in-one-command).

```bash
orchstep run setup            # detect OS, then install every package idempotently
orchstep run setup --dry-run  # preview the resolved plan, install nothing
orchstep menu                 # pick a task interactively
```

The steps only `echo`, so it is safe to run anywhere. To make it live, swap the
`install` echo for your real package-manager command:

- macOS: `brew install {{ loop.item }}`
- Linux: `sudo apt-get install -y {{ loop.item }}`

Add or remove tools by editing the `packages` list in `orchstep.yml` — the same
list runs on every machine.
