# conduit-not-vault

The conduit-model demo from the OrchStep blog post
[Secrets without leaks: the conduit model](https://orchstep.dev/blog/secrets-without-leaks-the-conduit-model).

```bash
orchstep run call            # both echoes print token=*** — the value is scrubbed
orchstep run call --dry-run  # plan shows the resolver but never runs it
```

The `cmd:` resolver is a `printf` stand-in so this runs anywhere. Swap it for your
own secret tool's CLI (`op read`, `vault kv get`, `aws secretsmanager get-secret-value`)
and the masking guarantees are identical.
