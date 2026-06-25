# reproducible-lockfile

The "reproducible modules with the lockfile" demo from the OrchStep blog. Pins a
remote module to an immutable commit + content hash in `orchstep.lock`.

    orchstep module lock      # write orchstep.lock (source/version/tag/commit/hash)
    orchstep module verify    # CI gate: re-fetch pinned commit, recompute hash
    orchstep module update    # re-resolve to newest allowed, re-pin
    orchstep run hello        # runs against the pinned commit, not the tag

Commit `orchstep.lock`. In CI, run `orchstep module verify` so a moved tag or a
tampered module fails the build instead of silently changing what runs.
