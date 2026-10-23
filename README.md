# Solar-Flare-Prediction-Enhanced
The "Enhanced Solar Flare Prediction" is a repository that improved version of the previous model (https://github.com/ZeinabHassani/SolarFlarePredition/).
This work applies the Enhanced Decomposition-LSTM (DLSTM) networks with STL decomposition to detect temporal quasi-patterns in regular flare time series from 2003 to 2023 recorded by GOES.

 # Keywords
Solar flare forecasting, Non-stationary time series, Decomposition, BiLSTM.

# Overview
The project includes the following:

   1. **Preprocessing and decomposition:** Smoothing, Normalization, Regularization, STL decomposition, and Oversampling Sliding Window
    
   2. **Solar flare forecasting:** integrates three prediction modules—trend, seasonal, and residual—along with a classification module.


# DataSet
The dataset includes a list of solar flare events from 2003 to 2023 that are obtained  from x-ray GOES data(https://doi.org/10.5281/zenodo.10560188). 
This work employs peak fluxes and waiting times of irregular flare time series. Also, the irregular flare time series is regularized  with a 3-hour interval  that contains maximum peak fluxes within each interval.

# Results


<img src="https://github.com/ZeinabHassani/Solar-Flare-Prediction-Enhanced/blob/main/Results/figure31.jpg" width="400" />

<img src="https://github.com/ZeinabHassani/Solar-Flare-Prediction-Enhanced/blob/main/Results/figure32.jpg" width="400" />
Accuracy (right panel) and TSS (left panel) of the EDLSTM-STL model obtained from 4-fold cross-validation.

<img src="https://github.com/ZeinabHassani/Solar-Flare-Prediction-Enhanced/blob/main/Results/figure40.jpg" width="400" />
The samples of confusion matrix elements for predicting the small and large flares. The sample of confusion matrix including T P = 9344, T N = 290, F N = 7, and F P = 447. The background images represent samples of large and small flares in the diagonals elements, respectively.

<img src="https://github.com/ZeinabHassani/Solar-Flare-Prediction-Enhanced/blob/main/Results/figure51.jpg" width="400" />
<img src="https://github.com/ZeinabHassani/Solar-Flare-Prediction-Enhanced/blob/main/Results/figure52.png" width="400" />

# Authors
[Zeinab Hassani](https://scholar.google.com/citations?user=tDYkBZMAAAAJ&hl=en), [Davud Mohammadpur](https://scholar.google.com/citations?user=f_JH18oAAAAJ&hl=en), and [Hossein Safari](https://scholar.google.com/citations?user=nCc1FV8AAAAJ&hl=en)


# Citation
If you find this repository useful, please cite our paper (https://link.springer.com/article/10.1007/s11227-026-08493-7):

     @article{Hassani2026,
     author = {Hassani, Zeinab and Mohammadpur, Davud and Safari, Hossein},
     doi = {10.1007/s11227-026-08493-7},
     issn = {1573-0484},
     journal = {The Journal of Supercomputing},
     number = {5},
     pages = {326},
     title = {{Non-stationary flare time series prediction using bidirectional long short-term memory based on STL decomposition}},
     url = {https://doi.org/10.1007/s11227-026-08493-7},
     volume = {82},
     year = {2026}
     }

