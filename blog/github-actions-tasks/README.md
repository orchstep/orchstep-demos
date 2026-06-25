# github-actions-tasks

Demo for the OrchStep blog post
[GitHub Actions without the YAML sprawl](https://orchstep.dev/blog/github-actions-without-the-yaml-sprawl).

```bash
orchstep run setup
orchstep run test --var suite=unit
orchstep run test --var suite=integration   # matrix-friendly
orchstep run build
```

The GitHub workflow stays thin and just calls these tasks. The steps only
`echo`, so the demo runs anywhere — swap them for your real commands.
