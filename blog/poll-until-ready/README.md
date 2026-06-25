# poll-until-ready

The "poll until ready, the right way" demo from the OrchStep blog.

    orchstep run release   # deploy -> settle (wait) -> bounded poll -> done

No unbounded `while`: the poll is a `count` loop with `delay` + `until`, so it
can never hang. Steps are `echo`/`wait` only, so it runs anywhere.
