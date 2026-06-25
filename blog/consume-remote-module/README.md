# consume-remote-module

The "consume a remote module from Git" demo from the OrchStep blog. Imports a
versioned module straight from a public Git repo and calls its exported task.

    orchstep module info github.com/orchstep/test-module-single   # show versions
    orchstep run hello            # resolve ^1.0.0 -> v1.1.0, fetch, run
    orchstep run hello --dry-run  # preview the plan, run nothing

The first run resolves `^1.0.0` to `v1.1.0`, caches it under
`~/.orchstep/cache/modules/`, and writes `orchstep.lock`.
