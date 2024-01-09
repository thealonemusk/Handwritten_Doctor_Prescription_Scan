# Handwriting Recognition with TensorFlow and Keras

This project focuses on Optical Character Recognition (OCR) using TensorFlow and Keras, aiming to recognize handwritten text from the IAM Handwriting dataset. The implemented pipeline includes data preprocessing, building a deep learning model, and evaluating its performance.

## Data Collection and Preparation

The notebook begins by fetching the IAM Handwriting dataset, organizing it into train, validation, and test subsets. The dataset contains handwritten words with associated labels.

## Data Input Pipeline

The data input pipeline involves preparing image paths, cleaning labels, and building character vocabularies. The dataset is processed to create TensorFlow `Dataset` objects, essential for training and validation.

## Resizing Images without Distortion

To maintain image aspect ratios and prevent distortion, a method for distortion-free resizing of images is introduced. It ensures that images are resized without altering their content, crucial for maintaining accuracy in recognition.

## Model Architecture

The OCR model is built using Convolutional Neural Networks (CNNs) combined with Recurrent Neural Networks (RNNs). The architecture involves several convolutional and LSTM layers, along with CTC (Connectionist Temporal Classification) loss as the endpoint layer.

## Training and Evaluation

The training phase involves setting up the model, defining callbacks for monitoring edit distances, and training the model on the prepared datasets. Evaluation metrics such as edit distance and precision are used to assess the model's performance.

## Inference and Visualization

The trained model is utilized to infer text from test samples. Visualizations are provided to showcase the model's predictions against the original text, offering insights into the model's accuracy.

## Custom Image Prediction

An additional functionality is demonstrated to predict text from custom images. The model's ability to handle external images is exhibited, highlighting its potential for real-world applications.

## Conclusion

The project concludes by emphasizing the model's compatibility with TensorFlow Lite for mobile applications and discussing potential enhancements, such as Spatial Transformer Networks, to improve alignment and performance for complex sequences.
