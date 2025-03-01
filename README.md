# Multi-Agent System for Speech Emotion Recognition and Classification


![newfwk](https://github.com/user-attachments/assets/c1ff5446-33c1-4b01-9e7e-b02f84b5e9c4)


Speech Emotion Recognition (SER) is a growing field that enables the identification of emotions from audio signals. This paper presents a multi-agent system implemented using CrewAI, designed to classify emotions in speech while ensuring modularity and scalability. The system is applied to the emoUERJ dataset, which contains emotional speech in Brazilian Portuguese. CrewAI orchestrates three specialized agents responsible for distinct tasks within the classification pipeline: preprocessing, feature extraction, and emotion classification. The Preprocessing Agent prepares audio data for analysis by removing noise, normalizing volume, and segmenting samples. The Feature Extraction Agent derives key acoustic features such as Mel-Frequency Cepstral Coefficients (MFCCs), Zero Crossing Rate (ZCR), and spectral energy, which are essential for distinguishing emotions like happiness, anger, sadness, and neutral. Finally, the Emotion Classification Agent evaluates three machine learning algorithms—k-Nearest Neighbors (kNN), Random Forest (RF), and Support Vector Machine (SVM)—to classify speech samples. Among these, SVM achieved the highest accuracy, demonstrating superior performance in emotion classification achieving 0.88, 0.86 and 0.87 in precision, recall and F1-score, respectively. This modular approach allows for seamless integration of new classification models and feature extraction techniques without disrupting the overall system. Future work will focus on expanding the dataset, integrating deep learning models, refining feature extraction techniques, and applying the system to other datasets to improve generalization.

DATASET:

- emoUERJ: https://zenodo.org/records/5427549

In the code `multiagent-system.ipynb`, its functionality is demonstrated using the emoUERJ dataset. To apply the process to other datasets, simply replace the dataset path in `data_path = '/content/drive/MyDrive/.../'`.
