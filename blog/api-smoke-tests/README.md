# api-smoke-tests

The endpoint smoke-test loop from the OrchStep blog post
[API smoke tests in five lines](https://orchstep.dev/blog/api-smoke-tests-in-five-lines).

```bash
orchstep run smoke
orchstep run smoke --var base=https://staging.api.example.com
```

The runnable demo `echo`s each request so it works offline. The blog post shows
the live `func: http` + `func: assert` version.
