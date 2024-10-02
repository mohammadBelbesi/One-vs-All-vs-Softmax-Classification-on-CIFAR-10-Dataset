# One-vs-All vs Softmax Classification on CIFAR-10 Dataset

## Project Overview
This project utilizes the **CIFAR-10 dataset**, a widely recognized dataset in the field of image classification. The CIFAR-10 dataset contains 50,000 labeled images distributed across 10 distinct classes (from 0 to 9). The goal of this project is to implement and evaluate the performance of **One-vs-All** classification and compare it to the **Softmax** classification method.

### Dataset Information
For this project, the CIFAR-10 dataset was preprocessed to generate:
1. **Features File**: Contains 16 features per image, specifically extracted for this task.
2. **Labels File**: Contains the class labels for each image, with values ranging from 0 to 9.

For more details on the CIFAR-10 dataset, visit the official [CIFAR-10 website](https://www.cs.toronto.edu/~kriz/cifar.html).

## Objective
The primary goal of this project is to implement a **One-vs-All classification** approach and evaluate its performance against the **Softmax** classification method. The models will be compared in terms of accuracy, runtime, cost function value, and F1 score.

## Project Tasks
1. **Comparison of One-vs-All and Softmax Approaches**  
   Implement both the **One-vs-All** and **Softmax** classification methods using the `LogisticRegression` class from the `sklearn` library. Compare the performance of the two methods based on:
   - **Accuracy**
   - **Runtime**

2. **Cost Function Calculation**  
   Compute the value of the **cost function** for each classification method to assess and compare model performance.

3. **F1-Score Evaluation**  
   Calculate the **F1-mean score** for each method to evaluate the balance between **precision** and **recall**.

4. **Confusion Matrix Analysis for One-vs-All Method**  
   Examine the **confusion matrix** for the One-vs-All method to identify any class pairs that are particularly challenging to distinguish.

5. **Focused Model for Challenging Class Pairs**  
   For one such challenging class pair, develop an additional model focused solely on distinguishing between these two classes. Integrate this specialized model into the classification pipeline as a fallback for when the initial model predicts one of these two classes. Evaluate whether the specialized model improves the overall classification performance for these classes.

## Dataset Splitting
The dataset is divided into:
- **70% for Training**
- **30% for Testing**

This division ensures a robust evaluation of model performance on unseen data.
