# changelog-release

The demo from the OrchStep blog post
[A real changelog and release, from the terminal](https://orchstep.dev/blog/a-real-changelog-and-release-from-the-terminal).

```bash
orchstep run release --var level=minor --dry-run   # preview the plan
orchstep run release --var level=minor             # bump, changelog, tag, build
```

The shell steps only `echo`, so it is safe to run anywhere — swap them for your
real changelog tool, `git tag`, and build commands to make it live.
