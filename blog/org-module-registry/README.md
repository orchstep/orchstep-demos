# org-module-registry

The "private module registry for your org" demo from the OrchStep blog. The
demo uses local module folders so it runs anywhere. In production you point a
`registries:` entry at your repo and pin versions with semver tags:

    registries:
      acme:
        url: github.com/acme/orchstep-modules
    modules:
      - { name: deploy, source: "@acme/deploy-kit", version: "^1.2.0" }
      - { name: notify, source: "@acme/notify-kit", version: "^0.4.0" }

Run the local version:

    orchstep run release            # ship using the shared modules
    orchstep run release --dry-run  # preview the plan, run nothing
