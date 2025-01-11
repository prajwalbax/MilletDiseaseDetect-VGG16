# Disease Detection in Finger Millet (Ragi) Plant Using VGG16

## Overview
Finger millet (locally known as **Ragi**) is a vital crop for millions due to its nutritional and ecological benefits. However, diseases affecting finger millet can drastically reduce yield and threaten food security. This project focuses on developing a **disease detection system** using **VGG16**, a state-of-the-art Convolutional Neural Network (CNN), to assist farmers and researchers in identifying diseases early and accurately.

---

## Features
- **State-of-the-Art CNN**: Leveraging the power of **VGG16** with transfer learning to classify diseases in finger millet plants.
- **High Accuracy**: Tailored fine-tuning and data augmentation strategies ensure precise disease detection.
- **User-Friendly Interface**: An intuitive interface for real-time disease diagnosis.
- **Scalable Solution**: Designed to be extensible for other crops and regions.

---

## Dataset
The dataset consists of high-quality images of finger millet plants captured under various conditions. The dataset is preprocessed with techniques such as:
- **Image Resizing**: Standardized to the input size of 224x224 for VGG16.
- **Data Augmentation**: Rotation, flipping, and brightness adjustments to simulate diverse field conditions and reduce overfitting.

---

## Methodology
### 1. **Model Architecture**
The VGG16 model, pre-trained on ImageNet, serves as the base model. Key steps include:
- Removing the top classification layer.
- Adding custom dense layers with **Global Average Pooling**.
- Incorporating **Batch Normalization** and **Dropout** to prevent overfitting.

### 2. **Transfer Learning**
The pre-trained weights of VGG16 are fine-tuned to specialize in recognizing diseases in finger millet plants.

### 3. **Training Process**
- Optimizer: **Adam** with a learning rate of 0.0001.
- Loss Function: **Categorical Crossentropy** for multi-class classification.
- Metrics: Accuracy.

### 4. **Evaluation**
The model was evaluated on a validation set with metrics such as:
- Accuracy

---

## Results
- **Accuracy**: Achieved **88.8%** accuracy on the validation set.
- **Insights**: DenseNet performed better in earlier trials, but VGG16 showed comparable results with lower computational requirements.

---

## How to Use
### 1. **Prerequisites**
Ensure you have the following installed:
- Python 3.7+
- TensorFlow
- OpenCV
- Flask/Streamlit (for the user interface)

### 2. **Steps to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/prajwalbax/MilletDiseaseVision---VGG16-.git
   ```
2. Navigate to the project directory:
   ```bash
   cd ragi-disease-detection
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the model:
   ```bash
   python app.py
   ```
5. Access the web app:
   Open your browser and navigate to `http://localhost:5000`.

---
## List of disease detected:
1. Healthy: 
   ![2a881a07eac63bfb5f1859283c7934a075e89888](https://github.com/user-attachments/assets/46f4f627-5b8e-4d62-977d-1e1266f14937)
   
2. Downy mildew:
   ![ff01a0f1b91af72971e678b3c7e77ff8ea1e3a62](https://github.com/user-attachments/assets/e08adffa-7be6-46b8-a7dd-bd3988526ead)
   
3. Mottle streak:
![4f5e8c462c7577a88bd11c821a41afb87d62b548](https://github.com/user-attachments/assets/92f8799e-6324-4467-b258-824e9d8397bb)

4. Seedling:
![89b01feecbda1be09c5ae083f586703980e2c939](https://github.com/user-attachments/assets/35d20be6-bbcc-40d7-bb40-09e2bab1fbd3)

5. Wilt:
![0620938489481050bac02b97ac21989b93abe6d2](https://github.com/user-attachments/assets/4462c786-00da-4b4e-89bf-071e79032896)

 6. Smut:
    ![a1cae5e80eef9cd9d9b3570a8c62b81b54af37b7](https://github.com/user-attachments/assets/5017763b-4513-4a9d-9e1a-3d45126410d5)





## Applications
- **Farmers**: Empower smallholder farmers with a tool to identify diseases early, reducing crop loss.
- **Researchers**: Aid agricultural researchers in understanding disease patterns.
- **Agricultural Extension Services**: Enhance extension officers' capacity to assist farmers.

---

## Future Work
- Expand the model to include more diseases and other crops.
- Incorporate Explainable AI (XAI) for better insights into predictions.
- Develop a mobile application for easier field use.

---

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a pull request.

---

## Acknowledgments
Special thanks to:
- The farmers and agricultural communities for their invaluable insights.
- Open-source contributors and the TensorFlow community for providing tools and resources.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
For questions, feedback, or collaboration, feel free to reach out:
- **Email**: your-email@example.com
- **LinkedIn**: [prajwalbax](https://www.linkedin.com/in/prajwal-bax/))
- **GitHub**: [prajwalbax](https://github.com/prajwalbax)

Let's empower sustainable agriculture together!

