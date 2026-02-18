# Agent Orchestra UI (Mock)

## v1 Simplification: tmux wall

This version intentionally strips the dashboard down to the core concept:

- one pane per agent
- each pane behaves like a remote tmux view
- per-pane command input (send-keys style)
- optional broadcast command controls

No aggregate KPIs, no heavy orchestration chrome.

## Run
```bash
python3 -m http.server 8091 --directory .
```

Open `http://localhost:8091`.

## Next step (backend hookup)
- map each pane to a real tmux session/pane
- stream pane output over websocket
- wire input to tmux `send-keys`
