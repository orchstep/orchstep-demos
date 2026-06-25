# architect-environments

The "OrchStep for solutions architects" demo from the OrchStep blog.

    orchstep run provision --env dev    # 1 replica
    orchstep run provision --env prod   # 6 replicas

One workflow, many targets, selected with `--env`. Steps are `echo`-only,
so the whole thing runs anywhere with no side effects.
