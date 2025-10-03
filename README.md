# Fire Detection using Deep Learning

This project is a deep learning-based system for detecting fire from images. The goal is to build an early fire detection solution that can be more accurate than traditional sensor-based approaches by analyzing visual data.

---

## Project Overview
The Fire Detection System is designed to:
- Classify images as **fire** or **no fire**.  
- Achieve high accuracy using a deep convolutional neural network (CNN).  
- Reduce false positives by using an attention mechanism with the base model.  
- Provide a foundation that can later be extended to real-time video surveillance.

---

## Features
- Binary image classification: **fire** vs **non-fire**.  
- Uses **InceptionV3** as the base CNN with transfer learning.  
- Includes a **spatial attention mechanism** to focus on important regions.  
- Dataset of fire and non-fire images (~3,000 images).  
- Achieved validation accuracy of **96.42%**.  

---

## System Workflow
1. Dataset of fire and non-fire images is collected.  
2. Images are preprocessed (resize, normalize, augment).  
3. Model built on InceptionV3 with custom dense layers + attention mechanism.  
4. Model is trained, validated, and tested.  
5. Predictions are made on new/unseen images.  

---

## Tech Stack
- **Programming Language**: Python  
- **Deep Learning Framework**: TensorFlow / Keras  
- **Model**: InceptionV3 with spatial attention mechanism  
- **Libraries**: NumPy, Pandas, Matplotlib, OpenCV (for preprocessing/visualization)  

---

## Challenges Addressed
- False positives from red/bright objects were common.  
  Added a spatial attention mechanism to help the model focus on the right regions.  
- Small dataset caused overfitting.  
  Solved using data augmentation and transfer learning.  
- Needed stable and high accuracy for safety-critical use.  
  Used InceptionV3 instead of training from scratch to get better performance.   

---

## Results
- Validation Accuracy: **96.42%**  
- Precision, Recall, F1 Score: ~0.95 

