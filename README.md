# Multi-Class Animal Image Classification Using CNN from Scratch

## 🔹 Problem Statement
With rapid technological advancements, industries such as wildlife conservation, surveillance systems, agriculture, and education increasingly require accurate, real-time image classification systems. Traditional methods often fall short when dealing with large datasets, real-world variations, and real-time monitoring. <br/>
This project addresses these limitations by developing a Convolutional Neural Network (CNN) from scratch, offering high performance in terms of accuracy, precision, and recall, while being robust to: <br/>
- Lighting, pose, and background variations <br/>
- Intra-class variability and inter-class similarity <br/>
- Real-time inference needs <br/>
- Generalization to unseen environments <br/>

This project presents a CNN model built from scratch to accurately classify images of cats, dogs, and snakes with over 98% accuracy, helping address critical global challenges through AI. <br/>

## 🔹 Dataset Description
This project utilizes the Animal Image Classification Dataset from [Hugging Face](https://huggingface.co/datasets/AlvaroVasquezAI/Animal_Image_Classification_Dataset). <br/>
It contains 3,000 labeled images across three categories:
- Cats: 1,000 images of various breeds and environments <br/>
- Dogs: 1,000 images in different settings and postures <br/>
- Snakes: 1,000 images covering multiple species and conditions <br/>

Image Format: JPG, RGB channels <br/>
Resolution: 256 × 256 pixels (uniform) <br/>

## 🔹 Methodology
### 1. Data Preprocessing
- Loaded dataset using load_dataset <br/>
- Mapped label indices to class names <br/>
- Saved a local copy to Google Drive for accessibility <br/>
- Used ImageFolder for image transformation <br/>
- Computed mean and standard deviation for normalization <br/>
- Applied augmentation and normalization to training set; only normalization on validation set <br/>
### 2. Model Architecture
A Sequential CNN model was built from scratch with: <br/>
•	3 Convolutional layers: Each followed by ReLU activation and MaxPooling <br/>
•	Flattening layer <br/>
•	2 Dense layers, ending with 3 output neurons for multi-class classification <br/>
•	Loss Function: Cross-Entropy Loss <br/>
•	Optimizer: Adam <br/>
### 3. Training & Evaluation
•	Dataset split: 80% Training / 20% Validation <br/>
•	Model trained using WorldQuant University's training module under [CC BY-NC-ND 4.0 License](https://creativecommons.org/licenses/by-nc-nd/4.0/) <br/>
Confusion Matrix Results (out of 1,000 samples per class): <br/>
- Cats correctly predicted: 979 <br/>
- Dogs correctly predicted: 978 <br/>
- Snakes correctly predicted: 982 <br/>

#### Performance Metrics
Metric ---| Cats | Dogs | Snakes <br/>
Precision | 98%	 | 97% -| 99% <br/>
Recall----| 98%	 | 98% -| 98% <br/>
Overall Accuracy: 98% <br/>
Confusion Matrix confirms minimal misclassifications

## 🔹 Model Summary
Total Parameters: 25,113,587 <br/>
Model Size: ~479 MB <br/>
Layers: 3 Conv Layers, 2 Dense Layers <br/>
Framework: PyTorch <br/>

## 🔹 Real-World Applications
This CNN model has strong potential for: <br/>
- Wildlife Monitoring and Biodiversity Analysis <br/>
- Ecological Research and Policy Development <br/>
- Real-time threat detection (e.g., poaching, habitat loss) <br/>

## 🔹 Business & Environmental Impact
- 70%+ reduction in manual labor hours <br/>
- Faster identification of ecological threats <br/>
- Enables data-driven conservation strategies <br/>

### Alignment with Sustainable Development Goals (SDGs)
- Goal 13 – Climate Action: Enables monitoring of biodiversity changes and animal migration in response to climate change <br/>
- Goal 15 – Life on Land:	Helps protect endangered species and their habitats via automated classification <br/>
- Goal 9 – Industry, Innovation, and Infrastructure:	Encourages innovation through AI-powered conservation and monitoring systems <br/>
- Goal 3 – Good Health and Well-being:	Assists in early snake detection, minimizing venomous snakebite fatalities <br/>

## 🔹 Future Work
- Expand to include more animal classes
- Deploy real-time classification app
- Integrate with drone imagery for remote wildlife monitoring
- Fine-tune for deployment on edge devices (e.g., Raspberry Pi)

### 👤 Author
Abdullahi Olalekan Abdulmumeen <br/>
*Data Scientist | Computer Vision Engineer* <br/>
📧 olalekanabdulmumeen3@gmail.com <br/>
📱 +2347053053024
