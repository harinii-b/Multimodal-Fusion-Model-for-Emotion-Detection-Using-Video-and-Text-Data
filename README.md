# Multimodal-Fusion-Model-for-Emotion-Detection-Using-Video-and-Text-Data

## Approach and Methodology

### 1. **Feature Engineering**
- **Visual Features**:
  - Used **OpenCV** and **Dlib** to extract facial features.
  - Employed **DeepFace** to analyze facial expressions.
- **Audio Features**:
  - Extracted **MFCC (Mel-frequency cepstral coefficients)** for voice emotion analysis.
  - Used **Librosa** for spectral feature extraction.
- **Text Features**:
  - Processed subtitle data using **NLTK** and **spaCy**.
  - Applied **BERT-based embeddings** to capture contextual meaning.

### 3. **Modeling and Multimodal Fusion**
- **Visual Model**:
  - Implemented a **CNN-based emotion detection model** for facial expressions.
- **Audio Model**:
  - Trained an **LSTM network** for emotion classification from voice features.
- **Fusion Strategy**:
  - Combined predictions from all three models using **late fusion techniques**.
  - Applied **attention mechanisms** to weigh different modalities dynamically.

### 4. **Evaluation Metrics**
- Used **F1-score**, **accuracy**, and **AUC-ROC** to evaluate the models.
- Compared unimodal and multimodal performances to validate fusion effectiveness.

## Results
- The **multimodal fusion model** outperformed unimodal approaches by **15-20%** in emotion detection accuracy.
- Achieved an **F1-score of 85%** across multiple emotion classes.
- Observed **significant improvements** in detecting subtle emotions (e.g., sarcasm, surprise) through text-video fusion.

## Challenges Faced
- **Synchronization Issues**: Aligning visual, audio, and subtitle timestamps.
- **Imbalanced Data**: Some emotions (e.g., joy and sadness) were overrepresented compared to others.
- **Complex Expressions**: Sarcasm and mixed emotions were difficult to classify.
