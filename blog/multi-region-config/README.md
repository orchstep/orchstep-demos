# multi-region-config

The "one config, many regions" demo from the OrchStep blog post
[Multi-region configuration](https://orchstep.dev/blog/multi-region-configuration).

```bash
orchstep run deploy --env eu-west-1       # one region, with its overrides
orchstep run deploy --env us-east-1       # primary region (more replicas)
orchstep run rollout                      # fan out across every region
orchstep run deploy --env eu-west-1 --dry-run
```

The region list lives in `vars.regions`; per-region policy lives in
`environments`. Steps only `echo`, so it is safe to run anywhere.
