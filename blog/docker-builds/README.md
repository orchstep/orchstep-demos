# docker-builds

The demo from the OrchStep blog post
[Docker builds you can actually read](https://orchstep.dev/blog/docker-builds-you-can-actually-read).

```bash
orchstep run build --var version=2.4.0   # build, tag, push (with retry), report
```

The steps only `echo`, so it is safe to run anywhere — swap the `echo`s for your
real `docker build` / `docker push` commands to make it live.
