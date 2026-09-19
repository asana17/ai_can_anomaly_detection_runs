# linear autoencoder against PCA

Printed output of three checks run by hand on 2026-09-14 and 2026-09-15, before runs
were recorded here. Each fits the linear autoencoder at every `k` and compares it with
PCA at the same `k`, since a linear autoencoder that has converged reaches the same
reconstruction error as PCA.

| file | what changes between fits |
|---|---|
| `linear_check_k2.log` | nothing, `k=2` at batch 1024 only |
| `linear_check_batch.log` | the batch, 256, 1024 and 4096 |
| `linear_check_rel.log` | the batch, 1024 and 4096, with training stopped on a relative improvement |

The table at the end of each file gives, per fit, the autoencoder's train and
calibration MSE and its threshold as ratios to PCA's. A ratio near 1 means the
autoencoder converged.

At `k=16` with batch 1024 the train ratio is 2.99 in `linear_check_batch.log` and 1.13
in `linear_check_rel.log`. Below `k=16` every ratio is within 2% of 1 in both. This is
what `BATCH` 1024 and the relative stopping test in
[models/docs/autoencoder.md](https://github.com/asana17/ai_can_anomaly_detection/blob/main/models/docs/autoencoder.md)
were chosen on.

Not known. The script and the commit were not kept. The stopping test of
`linear_check_batch.log` is taken to be an absolute one, from what was noted at the
time, not from the file. The data is an older split, 1760019 train rows against
3538312 in the current dataset.
