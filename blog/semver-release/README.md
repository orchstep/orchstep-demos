# semver-release

The "a semver release pipeline, end to end" demo from the OrchStep blog post
[A semver release pipeline, end to end](https://orchstep.dev/blog/a-semver-release-pipeline-end-to-end).

```bash
orchstep run publish --var channel=stable
orchstep run publish --var channel=beta --dry-run
```

`preflight` runs first as a called task. The `gate` step routes the artifact to
the stable or pre-release channel. Steps only `echo`, so it is safe to run
anywhere — swap the `echo`s for your real `git`, build, and publish commands.
