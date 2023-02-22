# Calibration-of-Neural-Networks

This repository contains the code for the first homework of the *Neural Networks for Data Science Applications* course (10589627), Sapienza University.

**TL;DR**: The task consisted of training, evaluating and improving the calibration of a *MLP* architecture, on a given dataset (i.e., *Wine Quality*), all using *TensorFlow*.

## Data

The dataset used is a well-known toy multiclass dataset concerning wine quality, and it is available for download at https://archive.ics.uci.edu/ml/datasets/wine+Quality.

## Calibration

The method for measuring the calibration of a model consisted of using *Confidence Histograms*, *Reliability Diagrams*, and the *Expected Calibration Error* (implementation details taken from Guo et al., 2017).

To improve the calibration instead the approach consisted of retraining the model from scratch using the Focal Loss (details in Mukhoti et al., 2020).

Lastly, in the final section there is an alternative approach to calibration to quantify uncertainty of a model, ie. Conformal Prediction. In this case i had to reproduce in TensorFlow a pseudocode taken from Angelopoulos and Bates, 2021.

## Results 
Everything is explained in the notebook `Calibration.ipynb`

## References
- Guo, C., Pleiss, G., Sun, Y., & Weinberger, K. Q. (2017, July). *On calibration of modern neural networks*. In International conference on machine learning (pp. 1321-1330). PMLR.
- Mukhoti, J., Kulharia, V., Sanyal, A., Golodetz, S., Torr, P., & Dokania, P. (2020). Calibrating deep neural networks using focal loss. Advances in Neural Information Processing Systems, 33, 15288-15299.
- Angelopoulos, A. N., & Bates, S. (2021). A gentle introduction to conformal prediction and distribution-free uncertainty quantification. arXiv preprint arXiv:2107.07511.
