# monorepo-tasks

The one-entry-point monorepo runner from the OrchStep blog post
[Tame your monorepo scripts](https://orchstep.dev/blog/tame-your-monorepo-scripts).

```bash
orchstep menu            # browse every package task
orchstep run build       # the single entry point — calls each package task
orchstep run web         # or run one package on its own
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `pnpm` / `turbo` commands to make it live.
