# Human Action Recognition (HAR)
### 📜 Introduction
This repository contains an implementation of a Human Action Recognition (HAR) model using two pretrained models. The goal is to classify 15 different human activities from images into their respective categories.

Key Features:
- 15 Activity Classes: Includes actions such as calling, cycling, dancing, etc.
- Dataset Size: 12k+ labeled images for training and 5,400 images for testing.
- Application: Useful in fields like surveillance, sports analytics, and healthcare.

### 🗂️ Dataset Details
#### Structure:

1. Train Folder:
   - Contains 15 subfolders, each representing a unique activity class (e.g., calling, clapping).
   - Each subfolder includes images related to that activity.
2. Test Folder:
   - ontains 5,400 unlabeled images to predict activity labels.
3. Testing_set.csv:
   - Lists the filenames of test images for submission format.
 4. Sample_submission.csv:
   - Provides a sample output format for predictions.

#### Classes:
  - Calling
  - Clapping
  - Cycling
  - Dancing
  - Drinking
  - Eating
  - Fighting
  - Hugging
  - Laughing
  - Listening to Music
  - Running
  - Sitting
  - Sleeping
  - Texting
  - Using Laptop



### 🛠️ Methodology
This project explores and compares two pretrained models as the backbone for feature extraction and classification:

  1. EfficientNetB7:
    Known for its efficiency in balancing model size and performance.
    Fine-tuned to adapt to the specific HAR dataset.
  2. VGG16:
    A classic, deeper architecture often used as a benchmark in image classification tasks.
    Fine-tuned to leverage its robust feature extraction capabilities.
    Workflow:

#### 🏆 Results and Comparisons
  Notes : Using kaggle gpu

| Model          | Training Accuracy | Training Time (Epochs)  | 
|-----------------|------------------|-------------------------|
| EfficientNetB7 | 97%               | 6 minutes (60 epochs)   | 
| VGG16          | 98%               | 7 minutes (60 epochs)   |


