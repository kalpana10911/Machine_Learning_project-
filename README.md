# Body Pose Recognition
## Abstract
Recognizing human body poses using BlazePose landmarks and machine learning classifiers for real-time applications in fitness, gaming, and surveillance.
- Recognize: stand, jump, duck, punch, throw, power, and kick. 
- Dataset from Kaggle – Body Pose Recognition
- Features: 33 body landmarks from BlazePose
- Machine learning Algorithms: Random Forest, SVM (Support Vector Machine), MLP (Multi-Layer Perceptron) 
- Goal: High accuracy + Real-time recognition

## ArCHITECTURE
- BlazePose (Mediapipe) as base architecture.
- Extracts 33 landmarks (x,y coordinates) from body images.
- Designed for real-time performance (30+ FPS on mobile devices).
- Accurate joint tracking; optimized for fitness/sports applications.
- Pre-trained → reduces training cost and improves generalization.

## Target PROBLEM
- **Goal:** Build a system that can automatically recognize and classify human body poses using landmark data.
- **Challenge:** Many poses look visually similar (e.g., sitting vs squatting).
Variations due to body size, camera angle, background, and lighting.

- **Need:** A robust model that can generalize well to real-world conditions.
- **Importance:** Enables gesture-based human–computer interaction.
Useful in fitness tracking, rehabilitation, sports analytics, and sign language recognition.

## Dataset
