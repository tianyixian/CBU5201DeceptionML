
# CBU5201DeceptionML Audio Story Veracity Detection

## Overview

This project aims to build a machine learning model that predicts whether a narrated story in an audio recording is true or false. The model takes as input audio recordings of 3-5 minutes in duration and outputs a binary classification of the story's authenticity.

## Dataset

The project utilizes the CBU5201 Deception Dataset, which consists of 100 audio recordings along with their corresponding Language and Story Type attributes. The dataset can be downloaded from:
- Audio recordings: https://github.com/CBU5201Datasets/Deception
- CSV file with attributes: https://github.com/CBU5201Datasets/Deception/blob/main/CBU0521DD_stories_attributes.csv

## Methodology

The project involves the following steps:

1. **Feature Extraction**: Extract audio features such as Mel-frequency cepstral coefficients (MFCC), zero-crossing rate, spectral centroid, and chroma features using the Librosa library.

2. **Data Preprocessing**: Normalize the audio data and encode the categorical attributes.

3. **Model Training**: Train a logistic regression model on the extracted features to classify the stories as true or false.

4. **Model Evaluation**: Evaluate the model using metrics such as accuracy, precision, recall, and F1 score.

5. **Ensemble Learning**: Build an ensemble model using a voting classifier to improve the model's generalization ability.

## Getting Started

To set up the project locally, follow these steps:

1. **Clone the Repository**:
   ```
   git clone https://github.com/yourusername/AudioStoryVeracityDetection.git
   cd AudioStoryVeracityDetection
   ```

2. **Install Dependencies**:
   ```
   pip install -r requirements.txt
   ```

3. **Download the Dataset**:
   - Download the audio files and the CSV file from the provided GitHub links.

4. **Run the Jupyter Notebook**:
   ```
   jupyter notebook CBU5201_miniproject.ipynb
   ```

## Project Structure

```
AudioStoryVeracityDetection/
│
├── data/                 # Directory for the dataset and audio files
│
├── notebooks/            # Jupyter notebooks for data analysis and model training
│   └── CBU5201_miniproject.ipynb
├── README.md             # This file
├── requirements.txt      # List of Python dependencies
└── .gitignore           # Git ignore file
```

## Evaluation

The model achieved an accuracy of 100% on the test set, indicating strong classification ability. However, due to the limited dataset, the model's generalization ability to new data requires further validation.

## Conclusion

The project demonstrates the potential of using audio features to classify the authenticity of stories. Further work includes expanding the dataset and exploring more complex models to improve the model's robustness and generalization.

## References

- Librosa Documentation: https://librosa.org/
- Scikit-learn Documentation: https://scikit-learn.org/

## Author

**Yixian Tian**
- Email: [tianyixian.nanshan@foxmail.com](mailto:tianyixian.nanshan@foxmail.com)

