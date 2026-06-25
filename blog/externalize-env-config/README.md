# externalize-env-config

The externalized env-config demo from the OrchStep blog post
[Externalize env config into files](https://orchstep.dev/blog/externalize-env-config-into-files).

```bash
orchstep run deploy                       # defaults.yml only
orchstep run deploy --env nonprod-dev     # defaults + nonprod + nonprod-dev
orchstep run deploy --env nonprod-staging # defaults + nonprod + nonprod-staging
orchstep run deploy --env prod-production # defaults + prod + prod-production
```

Each file is a flat map of values. The filename is the hierarchy: later, more
specific files override earlier ones. The steps only `echo`, so it runs anywhere.
