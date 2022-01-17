# DeepPulse
 An Uncertainty-aware Deep Neural Network for Heart Rate Estimations from Wrist-worn Photoplethysmography and Triaxial Accelerometer
 ## DATA
 - [IEEE SPC 2015](https://sites.google.com/site/researchbyzhang/ieeespcup2015)
 - [DaLia](https://archive.ics.uci.edu/ml/datasets/PPG-DaLiA)
 - [BAMI-II](https://github.com/hooseok/gyro_acc_ppg)
 ### Preprocesing:
 1. 2nd order Butterworth band-pass filter with cutoff frequencies of 0.5Hz-4.5Hz
 2. Resampled to 64Hz
 3. Normalized to zero mean and unit variance
 4. , Sliding window was applied with a window length of 8 seconds and a 2 second slide
 
 ## DeepPulse Architecture
![DeepPulse Architecture](https://github.com/danielray54/DeepPulse/blob/main/Images/DEEPPULSEARCH.png?raw=true)

## Results
| Method        | IEEE Train  | IEEE Test     | PPG-DaLiA   | BAMI-II     |
|---------------|-------------|---------------|-------------|-------------|
| Deep PPG      | 4.00 ± 5.40 | 16.51 ± 16.10 | 7.65 ± 4.20 | N/A         |
| CorNET (LOSO) | 4.67 ± 3.71   | 6.61 ± 5.35     | N/A         | N/A         |
| Binary CorNET | 6.20 ± 4.95   | 7.31 ± 6.14     | N/A         | N/A         |
| PPGnet        | 3.36 ± 4.10   | 12.48 ± 14.45   | N/A         | N/A         |
| Chung et al.  | 0.67 ± 0.50   | 0.86 ± 0.80     | N/A         | 1.46 ± 1.23 |
| DeepPulse     | 2.76 ± 2.95   | 5.05 ± 5.50     | 2.12 ± 3.09   | 2.38 ± 2.57   |
