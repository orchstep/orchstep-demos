# live-demo — watch the LIVE graph

`orchstep serve` here, select **deploy**, open the **RUN** tab, hit **▶ Run**, then
switch to the **LIVE** sub-tab. The `deploy` task sleeps 2-3s per step (~17s total)
so you can watch each node light up: queued → running (amber ▶) → done (green ✓),
the `gate` branch resolve, and the run complete. The `quick` task is instant for
comparison. To slow your own workflows, add `sleep N` to a step's `do:` (or use `func: wait`).
