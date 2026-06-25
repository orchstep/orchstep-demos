# company-module-registry

The "company module registry" demo from the OrchStep blog. Maps a company scope
to a monorepo with a `registries:` block, then imports `@mycompany/module1`.

    orchstep module lock          # resolve @mycompany/module1 -> tag module1/v1.0.0
    orchstep run main             # call the shared module's task
    orchstep run main --dry-run   # preview the plan, run nothing

The custom `@scope` only resolves because the `registries:` block lives in this
workflow. A bare `orchstep module resolve @mycompany/module1` would error
"unknown registry scope".

In your own org, swap the registry URL for your monorepo
(`github.com/your-org/platform-modules`). For a closed, license-gated private
registry (`orchstep module publish` / `list-private`), see OrchStep Pro:
https://orchstep.dev/pro
