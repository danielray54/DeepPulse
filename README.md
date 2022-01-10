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
