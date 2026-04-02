Intrusion Detection System using Machine & Deep Learning on Network Traffic Data
## Project Overview

This project develops a Network Intrusion Detection System (NIDS) using Machine Learning and Deep Learning techniques to detect malicious activities in network traffic. The system analyzes captured network packets and classifies them as normal or attack traffic, improving cybersecurity monitoring and threat detection.

The project compares multiple ML and DL models to determine the most effective approach for intrusion detection on real network traffic data.

## Objectives
Improve intrusion detection accuracy using advanced ML and DL models
Reduce false positives in network traffic classification
Compare ensemble and hybrid models for better detection performance
Evaluate models based on accuracy, precision, recall, and F1-score
## Dataset
Source: Network traffic captured using Wireshark
Traffic Types: IPv4 & IPv6 (encrypted and non-encrypted)
Total Packets: 17,650 TCP packets
Normal Traffic: 7,875 packets
Attack Traffic: 9,775 packets
Dataset Features
Feature	Description
time_stamp	Packet capture time
src_ip	Source IP address
dst_ip	Destination IP address
protocol	Network protocol
length	Packet size
src_port	Source port
dst_port	Destination port
tcp_flags	TCP flag information
label	Normal or Attack
## Data Preprocessing
Converted .pcapng to CSV using PyShark
Handled missing values using Forward Fill (ffill)
Applied Label Encoding for categorical features
Feature Scaling for numeric columns
Managed class imbalance using class weights
## Feature Selection
Correlation Analysis using heatmap
Feature Importance using Random Forest
Selected top 40% most important features for training
## Machine Learning Models
Random Forest (RF)
Support Vector Machine (SVM)
RF + SVM Hybrid Model
XGBoost
RF + GB + LR Stacking Model
Best ML Model

## Stacking Model (RF + GB + LR) achieved 97% accuracy.

## Deep Learning Models
LSTM (Long Short-Term Memory)
GRU (Gated Recurrent Unit)
CNN-LSTM
LSTM-GRU Hybrid Model
Graph Neural Network (GNN)
Best DL Model

## LSTM-GRU Hybrid Model achieved 95% accuracy.

## Results
Ensemble learning improved intrusion detection performance.
Hybrid deep learning models effectively captured sequential network traffic patterns.
Feature engineering significantly improved classification accuracy.
## Technologies Used
Python
Scikit-learn
TensorFlow / Keras
PyTorch
Pandas
NumPy
Matplotlib
Seaborn
Wireshark
PyShark

