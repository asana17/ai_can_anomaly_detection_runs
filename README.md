---
datasets:
- asana17/ai_can_anomaly_detection_data
---

# ai_can_anomaly_detection_runs

Runs of the detector comparison in
[asana17/ai_can_anomaly_detection](https://github.com/asana17/ai_can_anomaly_detection),
and the models quantized from them and the C code generated from those for the board.

| directory | added by | described in |
|---|---|---|
| `results/<start time>/` | one run of `evaluate.pc.run` | [evaluate/docs/run_record.md](https://github.com/asana17/ai_can_anomaly_detection/blob/main/evaluate/docs/run_record.md) |
| `quantize/<export time>/` | one run of `quantize.export` | [quantize/docs/export.md](https://github.com/asana17/ai_can_anomaly_detection/blob/main/quantize/docs/export.md) |
| `board/<generate time>/` | one run of `quantize.generate` | [quantize/docs/generate.md](https://github.com/asana17/ai_can_anomaly_detection/blob/main/quantize/docs/generate.md) |
| `checks/<date>-<name>/` | a check run by hand | its own `README.md` |

The format can change between commits, so read those pages at the `commit` in the
directory's `meta.json`.

The runs were fitted on
[asana17/ai_can_anomaly_detection_data](https://huggingface.co/datasets/asana17/ai_can_anomaly_detection_data).
`20260916-001002`, `20260916-064753`, `20260916-234726` and `20260919-025203` used its
revision `4cc59c1`.
