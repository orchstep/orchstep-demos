# terraform-guardrails

The "wrap terraform with guardrails" demo from the OrchStep blog post
[Wrap Terraform with guardrails](https://orchstep.dev/blog/wrap-terraform-with-guardrails).

```bash
orchstep run plan --var stage=production
orchstep run apply --var stage=production --dry-run   # preview every step, run nothing
orchstep run apply                                    # asks before it applies
```

`apply` always runs `fmt` and `validate` before `plan`, then gates the real
apply behind a confirm prompt. Steps only `echo`, so it is safe to run anywhere;
swap the `echo`s for real `terraform` commands to make it live.
