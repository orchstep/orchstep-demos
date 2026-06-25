# gitlab-ci-stages

Demo for the OrchStep blog post
[GitLab CI pipelines that read like intent](https://orchstep.dev/blog/gitlab-ci-pipelines-that-read-like-intent).

```bash
orchstep run build
orchstep run test
orchstep run deploy --var target=production
```

Each GitLab stage is one `orchstep run <task>`. The steps only `echo`, so the
demo runs anywhere — swap them for your real commands.
