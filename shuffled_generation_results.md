**Image reconstruction performance across EEG encoders.**  
Quantitative reconstruction performance averaged over two subjects with the UBP enabled. Metrics include low-level measures (PixCorr, SSIM, AlexNet(2)) and high-level semantic measures (AlexNet(5), Inception, CLIP, SwAV). Bold values indicate the best performance for each metric.

| EEG Encoder | PixCorr↑        | SSIM↑           | AlexNet(2)↑    | AlexNet(5)↑    | Inception↑     | CLIP↑          | SwAV↓          |
| :---------- | :------------- | :------------- | :------------- | :------------- | :------------- | :------------- | :------------- |
| Me          | 0.028±0.008     | 0.387±0.010     | 0.618±0.010     | 0.623±0.029     | 0.561±0.029     | 0.614±0.022     | 0.722±0.003     |
| Me(shuffled)| -.005±0.010     | 0.423±0.014     | 0.492±0.016     | 0.495±0.027     | 0.496±0.023     | 0.494±0.020     | 0.714±0.011     |
