# Body Pose Recognition
## Table of Contents

| Section | Link |
|--------|------|
| Abstract | [Go to Abstract](#abstract) |
| Architecture | [Go to Architecture](#architecture) |
| Target Problem | [Go to Target Problem](#target-problem) |
| Dataset | [Go to Dataset](#dataset) |
| Planned Methodology | [Go to Methodology](#planned-methodology) |

## Abstract
Recognizing human body poses using BlazePose landmarks and machine learning classifiers for real-time applications in fitness, gaming, and surveillance.

- Recognize: stand, jump, duck, punch, throw, power, and kick
- Dataset from Kaggle – Body Pose Recognition
- Features: 33 body landmarks from BlazePose
- Machine learning Algorithms: Random Forest, SVM (Support Vector Machine), MLP (Multi-Layer Perceptron)
- Goal: High accuracy + Real-time recognition


## Architecture
- BlazePose (Mediapipe) as base architecture
- Extracts 33 landmarks (x,y coordinates) from body images
- Designed for real-time performance (30+ FPS on mobile devices)
- Accurate joint tracking; optimized for fitness/sports applications
- Pre-trained → reduces training cost and improves generalization


## Target Problem
- **Goal:** Build a system that can automatically recognize and classify human body poses using landmark data.

- **Challenge:** Many poses look visually similar (e.g., sitting vs squatting).

Variations due to body size, camera angle, background, and lighting.

- **Need:** A robust model that can generalize well to real-world conditions.

- **Importance:** Enables gesture-based human–computer interaction.

Useful in fitness tracking, rehabilitation, sports analytics, and sign language recognition.


## Dataset
**Body Pose Recognition**

Dataset link:  
https://www.kaggle.com/datasets/rawatjitesh/body-pose-recognition

## Planned Methodology
### Preprocessing
- **Pose Extraction:** Use MediaPipe Pose to detect 33 body landmarks (x, y, z, visibility).

- **Feature Engineering:** Flatten landmark coordinates into feature vectors (e.g., 33 × 2 = 66 features)

- **Data Cleaning:** Handle missing landmarks (drop frames or impute values)

- **Normalization:** Scale coordinates relative to torso length/shoulder width to ensure size & position independence
### Model Setup
#### Architecture Choice:
- **Baseline:** ML classifiers (SVM, Random Forest) for simple pose classification

- **Advanced:** Deep Learning (CNN / LSTM / GCN) for sequential pose estimation & action recognition.

- **Training:** Split dataset into train, validation, test sets 

- **Optimization:** Use Adam/SGD with tuned hyperparameters
## Technologies Used

- Python
- OpenCV
- MediaPipe
- Scikit-learn
- TensorFlow / PyTorch
- NumPy
- Pandas




