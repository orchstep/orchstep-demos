# golden-paths

The "one sanctioned way to ship" demo from the OrchStep blog. The golden path
lives in a module, so every team gets the same build/verify/deploy steps.

    orchstep run release                          # ship the default service
    orchstep run release --var service=payments   # ship another service
    orchstep run release --dry-run                # preview the plan, run nothing
