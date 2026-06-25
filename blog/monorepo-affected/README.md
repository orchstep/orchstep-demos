# monorepo-affected

Demo for the OrchStep blog post
[Build only what changed in your monorepo](https://orchstep.dev/blog/monorepo-affected-builds).

```bash
orchstep run detect
orchstep run ci                               # build + test each affected package
orchstep run ci --dry-run                     # preview the per-package plan
```

`detect` reports the affected packages; `ci` loops over them and gates the
merge on the result. The list is static here so the demo runs anywhere — in a
real repo it comes from a git diff against the base branch. Steps only `echo`.
