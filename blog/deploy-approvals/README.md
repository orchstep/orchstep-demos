# deploy-approvals

The "deploy approvals and manual gates" demo from the OrchStep blog.

    orchstep run publish                          # human at terminal: prompts to confirm
    orchstep run publish --var approve=true       # skip the prompt, approve it
    ORCHSTEP_NON_INTERACTIVE=true orchstep run publish   # CI: default (false) auto-skips
    orchstep run publish --dry-run                # preview the plan, run nothing

Every step is echo-only, so it runs anywhere.
