# Agent Orchestra UI (Mock)

A lightweight, static mockup for managing multiple agents at once.

## What's in v0.2
- Fleet status overview (agent/state/task/cpu)
- Live event stream panel
- **Task delegation visualization**
  - Create task
  - Choose priority
  - Auto-route or direct assign to agent
  - Queue visualization updates in real-time
- **Per-agent checklist cards** for readiness/progress tracking

## Run locally
```bash
python3 -m http.server 8091 --directory .
```

Then open `http://localhost:8091`.

## Status
This is a UI mock only (no backend orchestration yet).
