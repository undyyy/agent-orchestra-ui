# Agent Orchestra UI (Mock)

## v2: tmux wall + dual-pane file awareness

This version keeps the simple tmux-wall idea but adds a second panel per agent:

- **Left:** remote tmux pane view + command input
- **Right:** file tree with change icons (`clean`, `added`, `modified`, `deleted`)

Why this works:
- terminal gives execution transparency
- file tree gives instant code-change context

## Run
```bash
python3 -m http.server 8091 --directory .
```

Open `http://localhost:8091`.

## Next backend step
- left panel: stream actual tmux pane output
- right panel: parse `git status --porcelain` into tree + status badges
