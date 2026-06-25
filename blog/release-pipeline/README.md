# release-pipeline

The "OrchStep for release managers" demo from the OrchStep blog.

    orchstep run cut --var version=1.5.0
    orchstep run ship --var version=1.5.0 --var tier=production

`ship` cuts the release, publishes with retries, verifies, and rolls back in a
`catch:` on failure. Steps are `echo`-only, so it runs anywhere with no side
effects.
