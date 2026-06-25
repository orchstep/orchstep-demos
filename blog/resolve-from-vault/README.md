# resolve-from-vault

The secret-resolver demo from the OrchStep blog post
[Resolve secrets from Vault, SOPS, or 1Password](https://orchstep.dev/blog/resolve-secrets-from-vault-sops-1password).

```bash
orchstep run migrate   # user and pass are pulled from one fetch, both masked as ***
```

The `cmd:` here is a `printf` stand-in returning the JSON shape a real tool emits;
`field:` navigates the parsed result. Replace it with `vault kv get -format=json`,
`op item get --output json`, or `sops -d` and nothing else changes.
