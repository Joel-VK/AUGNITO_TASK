# Emotion Classification Using Speech Signals

## Project Overview
This project aims to classify speech audio files into seven emotion categories: **Angry**, **Happy**, **Sad**, **Neutral**, **Fearful**, **Disgusted**, and **Surprised**. Emotion classification from speech signals is crucial for applications in human-computer interaction, therapeutic diagnostics, customer service automation, and sentiment analysis.

## Project Files
The models are organized across two Kaggle Notebooks:
- **`AUGNITO_SPEECH_TASK.ipynb`**: Contains the Wav2Vec2 Model for Sequence Classification.
- **`AUGNITO_SPEECH.ipynb`**: Contains the other three models, including the Hubert Large, WavLM with an enhanced classifier, and the ResNet18 model using spectrograms.

## Dataset
The dataset used for this project was obtained from [this Kaggle dataset](https://www.kaggle.com/datasets/uldisvalainis/audio-emotions/dataData) and uploaded into the Kaggle notebooks as a zip file. It contains 12,798 samples across seven emotion classes.

## Models
1. **Hubert Large Model**: A large transformer-based model that was effective but prone to overfitting on this dataset.
2. **Wav2Vec2 Model**: A base model, smaller than Hubert Large, which provided better generalization.
3. **WavLM with Enhanced Classifier**: Uses WavLM for feature extraction, followed by a custom classifier network for robust performance.
4. **ResNet18 on Mel Spectrograms**: Converts audio into mel spectrograms and leverages ResNet18 for classification.

## Results
Each model was evaluated on test accuracy, precision, recall, and f1-score, with Model 3 (WavLM with Enhanced Classifier) achieving the best accuracy and balanced performance across metrics.

## Future Directions
Planned improvements for this project include:
- **Expanding the dataset** to improve generalization.
- **Implementing data augmentation** techniques such as pitch shift and noise addition.
- **Applying regularization techniques** like early stopping, batch normalization, and tuning dropout rates.

## References
- Microsoft. *WavLM: A Unified Pre-trained Model for Speech and Audio Tasks*. 2021.
- Facebook AI. *Wav2Vec2: A Framework for Self-Supervised Learning of Speech Representations*. 2020.
- Facebook AI. *HuBERT: Self-Supervised Speech Representation Learning by Masked Prediction of Hidden Units*. 2021.

---

Please refer to the individual Kaggle notebooks for code, specific model configurations, and detailed results.
