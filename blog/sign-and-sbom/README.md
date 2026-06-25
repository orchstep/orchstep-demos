# sign-and-sbom

The "sign and SBOM every release" demo from the OrchStep blog.

    orchstep run attest                                  # sbom -> sign -> verify -> gate
    orchstep run attest --var image=ghcr.io/acme/api:2.0.0
    orchstep run attest --dry-run                         # preview the plan, run nothing

Every step is echo-only, so it runs anywhere.
