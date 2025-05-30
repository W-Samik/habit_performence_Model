# habit_performence_Model
# 🎯 Exam Score Predictor using TensorFlow

This project is an AI-powered model built using TensorFlow that predicts a student's **exam score** based on their **habits and lifestyle data**. It uses a neural network trained on a custom dataset to analyze patterns and make predictions.

## 📂 Dataset

The dataset `student_habits_performance.csv` includes various features related to students’ habits such as:

- Study hours
- Sleep schedule
- Class attendance
- Social media usage
- Physical activity
- Diet
- And more...

The **target variable** is the `exam_score`.

## 🧠 Model

The model is a **Sequential Neural Network** created using TensorFlow/Keras with the following structure:

- Input layer corresponding to the number of features
- One or more Dense hidden layers with ReLU activation
- Output layer predicting a single exam score (regression task)

### Example Architecture:
```python
model = tf.keras.Sequential([
    tf.keras.layers.Dense(64, activation='relu', input_shape=(input_dim,)),
    tf.keras.layers.Dense(32, activation='relu'),
    tf.keras.layers.Dense(1)  # Output: exam_score
])
