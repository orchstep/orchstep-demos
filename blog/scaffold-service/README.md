# scaffold-service

The demo from the OrchStep blog post
[Scaffold a new service in one command](https://orchstep.dev/blog/scaffold-new-services-in-one-command).

```bash
orchstep run new                              # prompts for the service name
orchstep run new --var service_name=billing   # no prompt — name supplied
```

The `render` steps build file contents into outputs (safe to run). Add
`args.output_file` to a `render` step to actually write the files to disk.
