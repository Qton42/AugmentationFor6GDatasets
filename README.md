# A Systematic Comparison between Data Augmentation Methods on 6G Datasets

Code for the [TU Delft](https://github.com/TU-Delft-CSE) [CSE3000 Research Project](https://github.com/TU-Delft-CSE/Research-Project) 2025/26 Q4, implemented for the paper:

Evaluating Tabular and Time-Series Data Augmentation for 6G-Relevant Network-Performance Regression

The datasets can be found here: https://doi.org/10.5281/zenodo.6907619

Tabular dataset - AMF performance

Time-series dataset - Python web server performance

## Abstract of the paper
Data-driven methods are expected to play an important role in future sixth-generation (6G) wireless systems, where network data can support performance prediction, simulation, and network optimization. However, collecting large and representative network-performance datasets can be difficult, which motivates the use of data augmentation. This study evaluates how different tabular and time-series augmentation techniques compare when addressing data scarcity in datasets relevant to future 6G systems. Two regression tasks are studied: a tabular AMF performance task using XGBoost and a time-series Python web-server performance task using an LSTM. Four tabular augmentation methods are evaluated: Gaussian Noise, SMOGN, CTGAN, and TVAE. Four time-series augmentation methods are evaluated: Jittering, Time Warping, TS-Mixup, and Frequency-domain augmentation. The methods are compared using downstream regression performance, statistical realism metrics, and diagnostic analysis of augmented data and test-set residuals. The results show that augmentation does not consistently improve regression performance. In the tabular task, all augmentation methods reduced performance compared with the XGBoost baseline. In the time-series task, Frequency-domain augmentation was the only method that improved the LSTM baseline, substantially reducing RMSE and MAE, although the final test-set R^2 remained negative. The diagnostics suggest that useful augmentation depends not only on preserving marginal distributions or value ranges, but also on preserving task-relevant feature-target relationships and temporal structure. Overall, the findings show that augmentation effectiveness is method- and data-type dependent, and that predictive performance should be evaluated together with statistical fidelity diagnostics.
