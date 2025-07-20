# 🧠 EEG Seizure Classification 


📁 Dataset
Source: Bonn University Epileptology Dataset

Samples: 500 recordings

Length: 23.5 seconds per sample (~4096 points)

Classes:

Sets Z, O, N, F: Non-seizure

Set S: Seizure

🧹 Preprocessing
Noise Reduction: Bandpass filter

Normalization: Mean = 0, Std = 1

Data Augmentation: Small noise added to enhance generalization

Missing Values: None found

🧪 Feature Extraction
Time-Domain:

Mean, Std, Variance, Skew, Kurtosis

Hjorth Parameters: Activity, Mobility, Complexity

Frequency-Domain:

Power Spectral Density across EEG bands (delta, theta, alpha, beta, gamma)

🧠 Models & Results
Model	Accuracy
Logistic Regression	79%
Decision Tree (depth=3)	88%
Support Vector Machine (linear)	80%
Random Forest (n=100)	96%
Neural Network (3-layer)	91%

Best Model: Random Forest (96%)

🧰 Tools Used
Python Libraries:

numpy, pandas – Data handling

scipy, sklearn – Modeling & metrics

tensorflow/keras – Neural networks

matplotlib, seaborn – Visualization

✅ Conclusions
Random Forest yielded the best performance.

Feature extraction from time + frequency domains improved accuracy.

EEG time series plots aided visual pattern recognition.

🚀 Future Work
Try advanced models: RNNs, CNNs, Transformers

Use wavelet transforms and time-frequency features

Apply to real-time seizure detection for healthcare solutions
