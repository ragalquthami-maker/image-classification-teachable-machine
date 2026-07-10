# image-classification-teachable-machine
Teachable Machine image classifier (earphones vs headphones) with Keras model and prediction script.
Earphones vs Headphones Image Classifier

An image classification model trained using Google's Teachable Machine (teachablemachine.withgoogle.com) to distinguish between earphones and headphones. The model was exported in TensorFlow/Keras format and tested using a Python script that loads the model and predicts the class of a new input image.

Project Files

- keras_model (1).h5: The trained image classification model, exported from Teachable Machine in TensorFlow → Keras format.
- labels (1).txt: Text file containing the class names (Earphones, Headphones).
- predict.py (or .ipynb): Python script that loads the model and labels, processes an input image, and predicts its class.
- training_evaluation.png: Screenshot of the model's accuracy per class from Teachable Machine.
- prediction_result.png: Screenshot of the script's output after running a prediction.

Steps Followed

1. Data Collection: Collected images of earphones and headphones from various sources, making sure to include different angles, colors, and backgrounds for better generalization.
2. Model Training: Uploaded the images into Teachable Machine under two classes (Earphones, Headphones) and trained the model using the platform's default settings.
3. Model Evaluation: Reviewed the accuracy per class using Teachable Machine's built-in evaluation tools to confirm the model was correctly distinguishing between the two classes.
4. Model Export: Exported the trained model in TensorFlow → Keras format, which generated two files: keras_model.h5 and labels.txt.
5. Prediction Script: Wrote a Python script that loads the trained Keras model and class labels, accepts an input image, resizes and normalizes it to match the model's expected input shape, runs a prediction, and prints the predicted class along with the confidence score.
6. Testing: Ran the script on Google Colab, uploading the model, labels, and a test image, then verified the output matched the expected class.

How to Run

1. Install the required libraries: pip install tf_keras pillow numpy
2. Make sure keras_model.h5, labels.txt, and the test image are in the same directory as the script.
3. Run the script: python predict.py
4. The script will print the predicted class and confidence score.

Results

See training_evaluation.png for the model's accuracy per class, and prediction_result.png for a sample prediction output.
