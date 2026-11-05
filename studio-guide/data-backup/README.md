# Set Bible data backup

Read-only export of the shared records behind the Red Mile Set Bible
(https://claude.ai/artifact/4xRxXwSDcz7S2bwNcxczri).

- `manifest.json` lists every collection, including the empty ones, with each document's version and last update.
- `<collection>/<doc_id>.json` holds each document's body exactly as stored.

| Collection | What it holds |
|---|---|
| `build` | The picked option for each light role and the camera Kelvin (`build/current`) |
| `status` | Purchase status per product: needed, ordered, arrived, rigged |
| `checks` | Ticked items on the rig-day, pre-show and Room today lists |
| `riglog` | Measured values from rig day |

To restore, write each file back to the same collection and document id with ArtifactData `set`.
Re-export after the team starts ticking items or logging measurements.
