# **ECG-Based Heart Disease Detection using CNN-Transformer**  

## **Overview**  
Heart diseases are among the leading causes of mortality worldwide, and early detection plays a crucial role in preventing severe complications. This project presents a deep learning-based approach to automatically classify heart diseases from ECG signals using a hybrid **CNN-Transformer** model. The combination of **Convolutional Neural Networks (CNN)** for feature extraction and **Transformer encoders** for sequential pattern learning allows the model to capture both spatial and long-range dependencies in ECG signals, leading to high classification accuracy.  

## **Features**  
- **High Performance on ECG Classification:**  
  - **Dataset 1:** Precision: **92%**, Recall: **90%**  
  - **Dataset 2:** Precision: **97%**, Recall: **99%**  
- **Hybrid Deep Learning Architecture:** Leverages CNN for local feature extraction and Transformer encoders for temporal dependencies.  
- **Data Augmentation with GANs:** To address class imbalance, we generated synthetic ECG signals for underrepresented classes using a **Generative Adversarial Network (GAN)**.  
- **Scalability:** Can be further trained on additional datasets for improved generalization.  

## **Model Architecture**  
Our model is designed to efficiently process ECG signals with:  
- **2 Convolutional Layers (CNN)**: Extracts spatial features from ECG signals to highlight critical patterns.  
- **5 Transformer Encoders**: Captures long-range dependencies and temporal relationships in the signal.  
- **Fully Connected Layers**: Used for classification based on the extracted features.  

## **Dataset**  
We used a publicly available ECG dataset from Kaggle:  
- **[Kaggle - Heartbeat Dataset](https://www.kaggle.com/datasets/shayanfazeli/heartbeat)**  
- This dataset contains ECG recordings categorized into different heart conditions, which were used for training and evaluating the model.  

### **Data Augmentation with GAN**  
One challenge in ECG classification is **class imbalance**, where some heart conditions have significantly fewer samples than others. To address this issue, we utilized a **Generative Adversarial Network (GAN)** to generate synthetic ECG signals for the minority classes. This approach helped improve the model's performance, particularly in rare conditions.  

## **Results**  
The model achieves high precision and recall across two different datasets, demonstrating its effectiveness in detecting heart diseases from ECG signals. The **GAN-based data augmentation** further improved the classification performance for underrepresented classes.  


## **Contributors**  
This project was developed by:  
- **Zahra Kazemi**  
- **Milad Tavakoli**  

If you find this project useful, feel free to contribute or reach out for collaboration!  
