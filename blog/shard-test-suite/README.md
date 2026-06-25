# shard-test-suite

The "shard your test suite for speed" demo from the OrchStep blog.

    orchstep run test                       # run all shards + gate
    orchstep run test --var total=8 --var shards='[1,2,3,4,5,6,7,8]'
    orchstep run test --dry-run             # preview the shard plan, run nothing

Every step is echo-only, so it runs anywhere.
