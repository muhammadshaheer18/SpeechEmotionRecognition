# SpeechEmotionRecognition
_________________________________________________________________________________

# Introduction:
In this project, the Toronto Emotional Speech Set (TESS) dataset is used to build a speech emotion recognition system. The TESS dataset contains audio recordings (2800) of actors speaking various sentences with different emotions, including anger, disgust, fear, happiness, neutral, and sadness. The goal is to develop a machine learning model that can accurately predict the emotional state of a person based on their speech.


# Data Preprocessing:
To prepare the data for training, first the TESS dataset is loaded using the librosa library. Then extract various features from each audio sample, including the mel-frequency cepstral coefficients (MFCCs), chroma features, and spectral contrast. These features are commonly used in speech recognition tasks and help to capture different aspects of the audio signal.


# Model Architecture:
A convolutional neural network (CNN) Long Short-Term Memory (LSTM) is used to classify the emotional state of each audio sample. The CNN consists of multiple convolutional layers followed by pooling layers and a fully connected layer. The input to the network is the feature matrix extracted from the audio samples, and the output is a probability distribution over the different emotions. The categorical cross-entropy loss function is used to train the model and the Adam optimizer to update the network weights.


# Training and Evaluation:
The TESS dataset is loaded into training, validation, and test sets, with 80%, 10%, and 10% of the data allocated to each set, respectively.The LSTM is trained on the training set for 50 of epochs and monitor the accuracy and loss on the validation set to prevent overfitting. Once the model converged, its performance on the test set is evaluated and report is formed for the overall accuracy as well as the precision, recall, and F1 score for each emotion.


# Conclusion:
In summary, A Speech Emotion Recognition system using the TESS dataset and a convolutional neural network (LSTM model). Model achieved a high accuracy on the test set, indicating that it can accurately predict the emotional state of a person based on their speech (taken in a real time input). This system could be useful in various applications, such as customer service chatbots, mental health monitoring, and speech therapy.
