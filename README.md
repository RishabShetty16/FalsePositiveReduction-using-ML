# FalsePositiveReduction-using-ML
Machine Learning-Based Intrusion Detection System
This repository contains the code for the machine learning model developed in the research paper, "Beyond Traditional IDS: A Comparative Study of Honeypot Integration and Machine Learning for False Positive Reduction." The primary goal of this project is to demonstrate the effectiveness of a machine learning-based Intrusion Detection System (IDS) in significantly reducing false positives compared to traditional IDS solutions.

Traditional Intrusion Detection Systems often suffer from high false positive rates, leading to alert fatigue and reduced security effectiveness. This project implements and evaluates a Random Forest classifier to identify malicious network traffic with high accuracy and precision, addressing this critical gap. The model is trained on a comprehensive dataset and demonstrates superior performance in distinguishing between benign and malicious activities. 

Methodology:The machine learning pipeline was designed to transform raw network traffic into actionable security insights.

Dataset
The model was trained using scenarios 50 and 54 from the CTU-13 extended dataset. This dataset is well-regarded for its realistic mix of normal background traffic and a wide range of malware communication and attack patterns. The data was split into 70% for training and 30% for validation. The model was tested using sceanrio 49

Feature Extraction
CICFlowMeter was used to convert raw packet captures (.pcap files) into a set of over 80 flow-based features suitable for machine learning. These features capture statistical properties of the traffic, such as flow duration, packet counts, and byte counts, which are crucial for identifying anomalous behavior.

We evaluated three different algorithms: Random Forest, XGBoost, and Logistic Regression. The Random Forest Classifier was selected as the primary model due to its superior performance.

