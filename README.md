# Classification of Hotel Booking Cancellations.

In the hotel business, booking cancellations by customers are a common and serious issue. They not only lead to a direct loss in revenue but also affect operational planning, resource allocation, and vacancy management. A sudden cancellation can result in rooms not being reassigned in time, causing resource waste. Therefore, early prediction of whether a booking will be canceled is extremely important, enabling hotels to take timely intervention measures.

The main objective of this study is to develop machine learning models capable of classifying and predicting whether a specific hotel booking will be canceled or not based on relevant booking information. Additionally, the goal is to apply these models to real-world scenarios to support practical prediction and decision-making in hotel operations.

## 🔄 Project Workflow

The overall workflow of this project follows a 5-step machine learning lifecycle, as illustrated below:

![Project Workflow](images/workflow.png)

## 📊 Problem Overview & Evaluation Metric

In this hotel booking classification task, the **target variable** indicates whether a reservation will be **canceled** or **not**.

Both types of prediction errors — **False Positives (FP)** and **False Negatives (FN)** — can cause losses for the hotel:

- ❗ **False Negatives (FN):** These are especially costly, as the hotel may **overbook** based on the incorrect assumption that some guests will cancel. If they don’t, the hotel may run out of rooms and lose potential customers.  
  → Therefore, **minimizing FN** (i.e., **maximizing Recall**) for the *cancellation* class is **critical**.

- ⚠️ **False Positives (FP):** These occur when the model predicts a cancellation, but the guest actually shows up. This could lead to **unnecessary overbooking** and **customer dissatisfaction**.

To balance both Precision and Recall, I use the **F1-score** as the primary evaluation metric.

> 🎯 **Key metric**:  
> The **F1-score of the *canceled* class** is the most important metric for evaluating model performance in this project.
