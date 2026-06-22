# orchstep serve — sandbox

A throwaway workflow for exploring the local web dashboard.

## Run it

```bash
cd /Users/mindbuger/data/git/orchstep/serve-sandbox
orchstep serve            # -> http://127.0.0.1:7777
# or pick a port:
orchstep serve --port 7799
```

Then open the URL in your browser.

## What to try

- **Launcher** — pick `deploy`, see its 5 steps + the variables (target / version / region), press **RUN**.
- **Live logs** — watch the log stream; toggle **follow**; hit **Cancel** mid-run on `long-job`.
- **FLOW tab** — switch to FLOW while `deploy` or `long-job` runs to watch nodes go amber → green live.
- **A failure** — run `flaky`: the `gate` step exits 1, so you get a FAILED run with a red node and the later step never runs.
- **Themes** — top-right: dark / blueprint / paper.
- **History** — every run is recorded; click back into any of them.

History is stored in `.orchstep/serve.db` (SQLite, this folder). Delete the
`.orchstep/` folder to reset.

## Edit & reload

Edit `orchstep.yml`, then just refresh the dashboard — it re-reads the file.
