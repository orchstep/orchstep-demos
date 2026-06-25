# render-config

The "render config files from templates" demo from the OrchStep blog.

    orchstep run config   # render one template per target (staging + production)
    orchstep run banner   # the render do: shorthand

Output goes to the run log; add `output_file:` to a render step to also write
a file. Steps here are render-only, so it runs anywhere.
