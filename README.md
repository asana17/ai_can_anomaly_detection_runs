# ai_can_anomaly_detection_runs

Runs of the detector comparison in
[asana17/ai_can_anomaly_detection](https://github.com/asana17/ai_can_anomaly_detection),
and the models exported from them for the board. Every directory is added by the
script that made it, and none is written to again.

| directory | added by | described in |
|---|---|---|
| `results/<start time>/` | one run of `evaluate.pc.run` | [evaluate/docs/run_record.md](https://github.com/asana17/ai_can_anomaly_detection/blob/main/evaluate/docs/run_record.md) |
| `board/<export time>/` | one run of `board.export` | [board/docs/export.md](https://github.com/asana17/ai_can_anomaly_detection/blob/main/board/docs/export.md) |

The format can change between commits, so read those pages at the `commit` in the
directory's `meta.json`.
