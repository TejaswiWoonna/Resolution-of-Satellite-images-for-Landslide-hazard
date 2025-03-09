# 🌍 Resolution of Satellite images for Landslide Hazard

## 📌 Overview
This project focuses on improving landslide detection using deep learning and high-resolution stereo satellite imagery. It aims to identify landslide features as small as 2–3 meters with advanced segmentation models.

## 🎯 Objectives
- **Improve Landslide Detection**: Utilize high-resolution satellite images for accurate segmentation.
- **Develop Deep Learning Models**: Implement U-Net, DeepLabV3+, and FCN-8 for landslide-prone area classification.
- **Evaluate Performance**: Use metrics like IoU, Precision, Recall, Dice Score, and F1-Score for model assessment.

## 📊 Dataset
We use the **LandslideSegNet dataset**, which contains **3960 high-resolution images** from various regions. The dataset consists of:
- **RGB satellite images (256×256 pixels)**
- **Binary masks indicating landslide regions**
- **Preprocessed and augmented data for model training**

## 🛠️ Methodology
1. **Data Preprocessing & Augmentation**
   - Resize images to **256×256**
   - Normalize pixel values
   - Apply **image augmentation** for dataset diversity

2. **Model Selection & Training**
   - **U-Net**: Captures fine-grained details for precise segmentation.
   - **DeepLabV3+**: Uses atrous convolution for multi-scale context analysis.
   - **FCN-8**: A simple and efficient fully convolutional network.

3. **Performance Evaluation**
   - Metrics: **IoU, Precision, Recall, Dice Score, F1-Score**
   - Fine-tune hyperparameters to avoid overfitting.

## 📈 Results
| Model        | Accuracy | Precision | Recall | Dice Score | mIoU |
|-------------|----------|-----------|--------|------------|------|
| **U-Net**   | 96.7%    | 70.2%     | 34%    | 45.8%      | 27.8% |
| **FCN-8**   | 96.2%    | 64%       | 35.4%  | 41.15%     | 28.16% |
| **DeepLabV3+** | 90.4% | 0%       | 0%     | 0%         | 0% |



## Dataset
https://www.kaggle.com/datasets/niyarrbarman/landslide-divided/data

