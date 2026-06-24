# orchstep-demos

Runnable example projects for OrchStep — used for local testing, the `serve`
dashboard, and documentation walkthroughs. Each subfolder is a self-contained
workflow you can `cd` into and run.

| Project | What it shows |
| --- | --- |
| `serve-demo/` | The `orchstep serve` dashboard end to end: a slow multi-stage `deploy`, **inline** `env_groups:` + `environments:` (Style 1, `--env dev/staging/production`), `dotenv:` (`environments/common.env` + optional `secrets.local.env?`), and a `--vars-file` example (`localtest/test_override.yml`). |
| `serve-multi-envs/` | **Externalized** env config (Style 2, `env_config:`): one file per environment under `environments/` (`defaults.yml` + `dev.yml`/`staging.yml`/`production.yml`), still selected with simple `--env dev`. |
| `serve-task-calls/` | A pipeline that **calls auto-discovered task files** under `tasks/` (incl. nested `tasks/deploy/`), with external env config. On the `serve` LIVE graph the run **descends into each called task** and lights up the whole chain. |
| `serve-sandbox/` | A minimal scratch workflow for quick experiments. |

> Style 1 (inline) and Style 2 (external `env_config:`) are mutually exclusive
> within one workflow — see /learn/environments. `serve-demo` shows inline;
> `serve-multi-envs` shows external. The engine errors if you declare both.

Each project keeps its own `.orchstep/` run state (git-ignored).
