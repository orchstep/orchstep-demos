# dry-run-preview

The "dry-run everything before you run it" demo from the OrchStep blog.

    orchstep run ship --dry-run                      # plan only, runs nothing
    orchstep run ship --dry-run --var target=production
    orchstep run ship --dry-run --open               # writes + opens an HTML plan
    orchstep run ship                                # run it for real, compare

Every step is an `echo`, so the plan's placeholders (like the build image tag)
become real values when you actually run it.
