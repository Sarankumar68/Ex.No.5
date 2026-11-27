# EXP 5 – Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

## 1. AIM

To compare different prompting techniques and evaluate their effectiveness in solving real-world engineering problems using the project **Crop Disease Detection Using Computer Vision**.

## 2. PROJECT TITLE

**Crop Disease Detection Using Computer Vision**

## 3. PROBLEM STATEMENT

Agriculture is one of the major sectors that supports human life and the economy. Crop diseases can significantly reduce agricultural productivity and cause financial losses to farmers.

Traditional crop disease identification requires manual inspection by agricultural experts. This process is time-consuming and may result in incorrect identification due to a lack of knowledge or experience.

To overcome these challenges, a computer vision-based system can be developed to automatically identify crop diseases from leaf images using image processing and deep learning techniques.

The proposed system analyzes uploaded crop leaf images, identifies disease symptoms and predicts whether the crop is healthy or affected by a particular disease.

## 4. SELECTED ENGINEERING SCENARIO

**Scenario:** Developing an automated crop disease detection system using computer vision and deep learning.

**Input:** Images of crop leaves captured using a mobile camera or uploaded by the user.

**Processing:** Image preprocessing, resizing, normalization, feature extraction and classification using a Convolutional Neural Network (CNN).

**Output:** Predicted crop disease name and classification result.

**Technologies Used:**
- Python
- OpenCV
- TensorFlow / Keras
- CNN (Convolutional Neural Network)
- NumPy
- Matplotlib
- Streamlit (for user interface)

## 5. BASE PROMPT (NAÏVE PROMPT)

**Prompt:**

Suggest a method to detect crop diseases using computer vision.

**AI-Generated Output:**

A crop disease detection system can be developed using computer vision and machine learning.

1. Collect images of healthy and diseased crop leaves.
2. Preprocess the images by resizing and normalizing them.
3. Train a CNN model using the collected dataset.
4. Use the trained model to classify crop leaf images.
5. Display the predicted disease name to the user.

This system helps farmers identify crop diseases quickly and efficiently.

## 6. IMPROVED PROMPTS USING DIFFERENT PROMPTING TECHNIQUES

### Technique 1 – Zero-Shot Prompting

**Prompt:**

You are an AI system development assistant. Explain how to develop a crop disease detection system using computer vision without providing any examples. Describe the dataset requirements, image preprocessing steps, CNN architecture, training process and prediction procedure. Suggest suitable Python libraries and explain how the system can help farmers identify crop diseases.

**AI-Generated Output:**

A crop disease detection system can be developed using a CNN-based image classification approach.

1. Dataset Collection: Collect images of healthy and diseased crop leaves from publicly available datasets such as PlantVillage.
2. Image Preprocessing: Resize images to 224 × 224 pixels, normalize pixel values and apply data augmentation.
3. Model Development: Build a CNN containing convolutional, ReLU, pooling and fully connected layers.
4. Model Training: Train the model using labeled images and categorical cross-entropy loss.
5. Evaluation: Evaluate the model using accuracy, precision, recall and F1-score.
6. Prediction: Allow users to upload leaf images and predict the corresponding disease class.

Python libraries such as TensorFlow, Keras, OpenCV and NumPy can be used.

### Technique 2 – Few-Shot Prompting

**Prompt:**

Develop a crop disease detection system using computer vision. Follow the examples below to understand the expected classification format.

Example 1:
Input: Healthy tomato leaf image.
Output: Healthy Tomato Leaf.

Example 2:
Input: Tomato leaf with yellow spots and brown lesions.
Output: Possible Early Blight.

Example 3:
Input: Potato leaf with dark irregular patches.
Output: Possible Late Blight.

Now explain how to develop a system that classifies crop leaf images into healthy and diseased categories. Include dataset collection, preprocessing, CNN training and prediction.

**AI-Generated Output:**

A crop disease detection system can be developed using supervised deep learning.

1. Collect labeled images of healthy and diseased crop leaves.
2. Organize images into separate classes such as Healthy, Early Blight and Late Blight.
3. Resize all images to a fixed dimension and normalize pixel values.
4. Apply data augmentation techniques such as rotation, flipping and zooming.
5. Train a CNN model using labeled training images.
6. Use the trained model to classify new leaf images.

Example prediction format:

| Input Image | Predicted Output |
|---|---|
| Healthy tomato leaf | Healthy Tomato |
| Tomato leaf with brown lesions | Possible Early Blight |
| Potato leaf with dark patches | Possible Late Blight |

The system can provide automated disease classification and reduce manual inspection efforts.

### Technique 3 – Persona Pattern

**Prompt:**

Act as an experienced Computer Vision Engineer and Deep Learning Researcher. You are assigned to develop an automated crop disease detection system for farmers.

Design a practical solution using CNN and Python. Explain the dataset requirements, image preprocessing techniques, model architecture, training procedure, evaluation metrics and deployment process. Also discuss the challenges involved in implementing the system in real agricultural environments.

**AI-Generated Output:**

As an experienced Computer Vision Engineer, I recommend developing a CNN-based crop disease classification system.

1. Dataset: Use a labeled dataset such as PlantVillage containing healthy and diseased leaf images.
2. Preprocessing:
   - Resize images to 224 × 224.
   - Normalize pixel values between 0 and 1.
   - Remove corrupted images.
   - Apply augmentation to improve model generalization.
3. Model Architecture:
   - Input layer
   - Convolutional layers
   - ReLU activation
   - Max pooling layers
   - Flatten or Global Average Pooling
   - Dense classification layer
   - Softmax activation
4. Training: Train the model using Adam optimizer and categorical cross-entropy loss.
5. Evaluation: Measure accuracy, precision, recall, F1-score and confusion matrix.
6. Deployment: Develop a simple web application using Streamlit.

Challenges include variations in lighting, leaf orientation, background noise, overlapping leaves and visually similar disease symptoms.

A transfer learning model such as MobileNetV2 can also be considered to improve performance and reduce computational requirements.

### Technique 4 – Chain-of-Thought Prompting

**Prompt:**

Analyze the engineering problem of crop disease detection using computer vision systematically. Explain the solution in a structured sequence covering problem identification, dataset selection, image preprocessing, feature extraction, CNN model design, training, evaluation and deployment. For each stage, explain its purpose, the method selected and the expected outcome. Include appropriate evaluation metrics.

**AI-Generated Output:**

A systematic approach to crop disease detection involves the following stages.

**Step 1: Problem Identification**

Manual disease identification is time-consuming. An automated image classification system can reduce the time required to identify visible crop disease symptoms.

**Step 2: Dataset Selection**

Collect labeled images of healthy and diseased leaves. PlantVillage is a suitable starting dataset.

**Step 3: Image Preprocessing**

Resize images to a fixed size, normalize pixel values and apply augmentation. This ensures consistent input for the model.

**Step 4: Feature Extraction**

CNN convolutional layers automatically extract important features such as spots, edges, discoloration and texture patterns.

**Step 5: Model Development**

Develop a CNN using convolutional layers, ReLU activation, pooling layers and fully connected layers.

**Step 6: Model Training**

Divide the dataset into training, validation and testing sets. Train the model using an appropriate optimizer and loss function.

**Step 7: Model Evaluation**

Evaluate performance using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

**Step 8: Deployment**

Develop a user-friendly application that accepts leaf images and displays the predicted disease class and confidence score.

The final system provides an automated approach for identifying visible crop disease symptoms.

### Technique 5 – Role-Based and Constraint-Based Prompting

**Prompt:**

Act as a professional AI engineer. Design a low-cost crop disease detection system for farmers using Python, OpenCV and CNN.

Consider the following constraints:

- The system should use publicly available datasets.
- It should work with images captured using mobile cameras.
- The model should be computationally efficient.
- It should classify multiple crop disease categories.
- It should provide prediction results with confidence scores.
- The system should be deployable using a simple web interface.

Suggest a suitable architecture, preprocessing methods, training strategy, evaluation methods and deployment approach.

**AI-Generated Output:**

A lightweight crop disease detection system can be developed using transfer learning with MobileNetV2.

1. Dataset: Use publicly available labeled crop leaf datasets.
2. Preprocessing: Resize images to 224 × 224 pixels and apply the preprocessing function required by MobileNetV2.
3. Data Augmentation: Apply rotation, horizontal flipping, zooming and brightness variation.
4. Model Architecture: Use MobileNetV2 as the feature extraction backbone and add a classification layer for disease categories.
5. Training: Freeze the pretrained layers initially and train the classification head. Fine-tune selected layers if necessary.
6. Evaluation: Measure accuracy, precision, recall, F1-score and inference time.
7. Deployment: Use Streamlit to create an interface where farmers can upload leaf images and view predictions.

The system should also include an unknown or uncertain prediction option when the confidence score is low. Real-world images should be used during testing to evaluate performance under different lighting and background conditions.

## 7. COMPARISON OF PROMPTING TECHNIQUES

| Prompting Technique | Quality | Accuracy | Depth |
|---|---|---|---|
| Naïve Prompt | Basic | General information | Low |
| Zero-Shot | Good | Relevant technical suggestions | Medium |
| Few-Shot | Good | Follows provided examples | Medium |
| Persona Pattern | Very Good | Engineering-focused suggestions | High |
| Chain-of-Thought | Very Good | Structured explanation | High |
| Role-Based and Constraint-Based | Excellent | Considers project requirements | Very High |

## 8. EVALUATION TABLE

The following scores are illustrative qualitative evaluations of the generated sample responses.

Scores are assigned on a scale of 1 to 5.

| Evaluation Criteria | Naïve | Zero-Shot | Few-Shot | Persona | Chain-of-Thought | Constraint-Based |
|---|---:|---:|---:|---:|---:|---:|
| Relevance | 3 | 4 | 4 | 5 | 5 | 5 |
| Accuracy | 3 | 4 | 4 | 4 | 4 | 5 |
| Completeness | 2 | 4 | 4 | 5 | 5 | 5 |
| Clarity | 4 | 4 | 4 | 5 | 5 | 5 |
| Feasibility | 3 | 4 | 4 | 5 | 5 | 5 |
| Usefulness | 2 | 4 | 4 | 5 | 5 | 5 |
| **Total** | **17** | **24** | **24** | **29** | **29** | **30** |

## 9. ANALYSIS AND OBSERVATIONS

The experiment demonstrates that the quality of AI-generated responses depends significantly on how the prompt is structured.

1. Naïve Prompting: Produces a basic solution but lacks technical details and implementation guidance.
2. Zero-Shot Prompting: Provides useful technical information without requiring examples.
3. Few-Shot Prompting: Helps the AI understand the expected classification format through examples.
4. Persona Pattern: Produces more professional and engineering-oriented responses by assigning a specific role to the AI.
5. Chain-of-Thought Prompting: Organizes the solution into logical stages, making the engineering process easier to understand.
6. Constraint-Based Prompting: Produces practical solutions by considering computational efficiency, deployment requirements and real-world limitations.

### Does ChatGPT consistently provide better results with improved prompts?

Yes, in this experiment, improved prompts generally produced more detailed, structured and relevant responses. However, a simple prompt can also produce a satisfactory answer when the problem is straightforward and the expected output is limited.

## 10. FINAL SELECTED PROMPTING TECHNIQUE

**Selected Technique: Role-Based and Constraint-Based Prompting**

This technique was selected because it provides a practical engineering solution while considering the project's technical requirements and real-world constraints.

It generates detailed information about dataset selection, preprocessing, model architecture, training, evaluation and deployment.

## 11. REFINED / FINAL PROMPT

Act as an experienced Computer Vision Engineer and Deep Learning Researcher.

I am developing a final-year engineering project titled "Crop Disease Detection Using Computer Vision".

The objective is to develop an automated system that identifies healthy and diseased crop leaves using image classification.

Design a complete and practical implementation using Python, OpenCV, TensorFlow/Keras and CNN.

Consider the following requirements:

1. Use publicly available datasets such as PlantVillage.
2. Explain image preprocessing, resizing, normalization and data augmentation.
3. Suggest an efficient CNN or transfer learning architecture such as MobileNetV2.
4. Explain model training, validation and testing.
5. Include suitable evaluation metrics such as accuracy, precision, recall, F1-score and confusion matrix.
6. Explain how to classify new crop leaf images.
7. Suggest a simple deployment method using Streamlit.
8. Consider real-world challenges such as lighting variations, background noise and visually similar diseases.
9. Provide a modular implementation plan and explain the purpose of each module.

Provide the solution in a structured engineering format with practical implementation details.

## 12. ENGINEERING VALIDATION

The proposed solution can be validated through the following steps:

1. Dataset Validation: Verify that the dataset contains correctly labeled healthy and diseased crop leaf images.
2. Preprocessing Validation: Check that all images are resized and normalized correctly.
3. Model Validation: Train the CNN model and monitor training and validation loss.
4. Performance Validation: Evaluate the trained model using an independent test dataset.
5. Classification Validation: Test the model using new leaf images that were not included in training.
6. Real-World Validation: Test images captured under different lighting conditions and backgrounds.
7. Deployment Validation: Verify that the application accepts images and displays the predicted class and confidence score correctly.

**Expected Outcome:** The system should identify crop disease categories with satisfactory classification performance. Actual accuracy and reliability must be established through experimental testing rather than assumed in advance.

## 13. CONCLUSION

Thus, different prompting techniques were applied to the engineering problem of crop disease detection using computer vision. The generated responses were compared based on relevance, accuracy, completeness, clarity, feasibility and usefulness.
