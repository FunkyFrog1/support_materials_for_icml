- **Self\-memory\-guidance:** We will present the performance obtained when the ViG module uses memory EEG itself as Q, K, and V, serving as a performance reference baseline to illustrate the system’s behavior in the absence of external perceptual guidance.

- **Shuffled\-visual\-Guidance:** We will conduct **shuffled guidance** experiments, testing the performance changes of MeViG when the auxiliary perceptual EEG comes from images of **different categories** from the memory content. This design covers the core scenarios of “erroneous guidance” or “mismatched guidance” mentioned by the reviewer. We expect that under this condition, the positive effects of the guidance module will be significantly weakened or may even cause interference. This experiment will directly answer your question about “whether MeViG can still improve performance under erroneous guidance.”

**Table: Memory EEG retrieval with VG module (ViT\-B/32).** Results are reported for each subject and their average, using different EEG sources for guidance.

| Guidance strategy | Sub 1 Top\-1 | Sub 1 Top\-5 | Sub 1 mAP | Sub 2 Top\-1 | Sub 2 Top\-5 | Sub 2 mAP | Avg Top\-1 | Avg Top\-5 | Avg mAP |
|-------------------|-----------------|-----------------|---------------|-----------------|-----------------|---------------|---------------|---------------|-------------|
| No-guidance | 3.60 ± 0.86 | 12.20 ± 1.94 | 9.94 ± 0.43 | 5.10 ± 0.92 | 18.90 ± 3.34 | 13.24 ± 1.19 | 4.35 ± 1.16 | 15.55 ± 4.32 | 11.59 ± 1.87 |
| Self-memory-guidance | 4.70 ± 1.68 | 12.20 ± 1.53 | 10.47 ± 1.09 | 5.60 ± 1.81 | 19.30 ± 2.71 | 13.61 ± 1.53 | 5.15 ± 1.72 | 15.75 ± 4.28 | 12.04 ± 2.08 |
| Shuffle-visual-guidance | 2.50 ± 0.79 | 11.30 ± 1.25 | 8.82 ± 0.30 | 6.50 ± 1.50 | 17.10 ± 0.82 | 13.42 ± 0.96 | 4.50 ± 2.39 | 14.20 ± 3.22 | 11.12 ± 2.52 |


**Table: Memory EEG retrieval with VG module (ViT\-H/14).** Results are reported for each subject and their average, using different EEG sources for guidance.

| Guidance strategy | Sub 1 Top\-1 | Sub 1 Top\-5 | Sub 1 mAP | Sub 2 Top\-1 | Sub 2 Top\-5 | Sub 2 mAP | Avg Top\-1 | Avg Top\-5 | Avg mAP |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| No-guidance | 3.10 ± 1.36 | 14.10 ± 1.32 | 9.84 ± 1.19 | 6.70 ± 1.94 | 19.70 ± 1.69 | 14.50 ± 1.05 | 4.90 ± 2.46 | 16.90 ± 3.18 | 12.17 ± 2.59 |
| Self-memory-guidance | 2.70 ± 0.57 | 14.10 ± 1.19 | 9.72 ± 0.39 | 6.70 ± 1.75 | 18.5 ± 2.55 | 14.08 ± 1.63 | 4.70 ± 2.44 | 16.30 ± 2.98 | 11.90 ± 2.56 |
| Shuffle-visual-guidance | 1.9 ± 1.03 | 11.9 ± 1.39 | 7.99 ± 0.79 | 5.10 ± 1.29 | 17.1 ± 0.22 | 12.5 ± 0.85 | 3.50 ± 2.01 | 14.50 ± 2.90 | 10.25 ± 2.50 |

**Table: Memory EEG retrieval with VG module (ViT\-bigG/14).** Results are reported for each subject and their average, using different EEG sources for guidance.

| Guidance strategy | Sub 1 Top\-1 | Sub 1 Top\-5 | Sub 1 mAP | Sub 2 Top\-1 | Sub 2 Top\-5 | Sub 2 mAP | Avg Top\-1 | Avg Top\-5 | Avg mAP |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| No-guidance | 4.00 ± 1.10 | 11.90 ± 1.24 | 9.74 ± 0.90 | 4.70 ± 0.51 | 15.30 ± 1.66 | 11.94 ± 0.55 | 4.35 ± 0.92 | 13.60 ± 2.24 | 10.84 ± 1.33 |
| Self-memory-guidance | 3.50 ± 0.50 | 12.40 ± 1.39 | 9.46 ± 0.45 | 4.90 ± 0.96 | 16.00 ± 1.46 | 12.55 ± 1.05 | 4.20 ± 1.03 | 14.20 ± 2.32 | 11.00 ± 1.80 |
| Shuffle-visual-guidance | 2.80 ± 0.91 | 11.50 ± 2.62 | 8.73 ± 1.02 | 3.70 ± 1.79 | 13.90 ± 2.04 | 10.43 ± 1.80 | 3.25 ± 1.42 | 12.70 ± 2.55 | 9.58 ± 1.60 |
