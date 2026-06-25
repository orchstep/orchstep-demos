# retries-and-timeouts

The "retries and timeouts as syntax" demo from the OrchStep blog.

    orchstep run publish   # push (retry + timeout + total_timeout) -> smoke -> done

The echoes succeed, so no attempt is wasted - the point is the shape: exact
field names `max_attempts`, `interval`, `backoff_rate`, `max_delay`, plus
`timeout` and `total_timeout`. Runs anywhere.
