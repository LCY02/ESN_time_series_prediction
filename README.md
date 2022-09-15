# ESN_time_series_prediction
This repository contains codes that implement echo state network (ESN) models for time series (signal) prediction.

**Data:**  `2sin.txt` `lorenz.txt`
**Codes:**  `ESN.ipynb`

**First part of the project**
Implement a standard echo state network (ESN) model. Do not include feedback from the output and do not use leaky-integrator neurons. Implement training of the read-out weights by means of the standard regularized least-square method. Perform some preliminary simulations by considering a _k_ step ahead forecasting task (evaluate several values of *k*, the forecasting horizon) on the "2sine" and "lorentz" time series (provided in the archive together with the notebook) and describe the experimental results. Note that, in order to train ESNs, you will have to create input-output pairs starting from the time series.
    
**Second part of the project**
Implement a version of the ESN model that is trained online by means of gradient descent (update weights after the presentation of each input data point). Perform simulations to compare the performance on k-step ahead forecasting tasks with respect to the standard ESN implementation (first part of the project) using the same time series. In the experiments, take again into account multiple _k_ values for the forecasting horizon (i.e., explore and comment on the effects of increasing *k* on the performance) and process the "2sine" and "lorenz" time series. Fine tune all hyper-parameters that significantly affect the performance and provide comments on their setting.

**Optional part of the project**
Implement the online training algorithm known as FORCE learning. The algorithm is described in "Sussillo and Abbott, *Generating Coherent Patterns of Activity from Chaotic Neural Networks*, Neuron 2009". Benchmark the resulting ESNs on the same two time series used before and comment the results with respect to the other two training algorithms.
