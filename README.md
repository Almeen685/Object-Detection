Road Condition and Direction Detection on Gilgit Roads using YOLOv5
Introduction
This project focuses on developing an object detection model to identify road conditions and directions on the challenging roads of Gilgit. Leveraging the YOLOv5 model, the goal is to detect turns (left, right), straight roads, and unexpected obstacles to improve safety and assist autonomous navigation systems. This real-time detection of road conditions supports applications in autonomous driving, driver assistance systems, and road monitoring.

Objective
The primary objective is to build an accurate and efficient object detection model for recognizing different road types and conditions from images. This includes:

Preprocessing the image data.
Implementing YOLOv5 for object detection.
Training and fine-tuning the model on labeled road data.
Evaluating model performance and visualizing results.
Dataset
The dataset, sourced from Roboflow, includes labeled images from Gilgit roads in four categories: straight, left turn, right turn, and unexpected obstacles.

Data Division:
Training Set: 70% of images.
Validation Set: 15% of images.
Test Set: 15% of images.
Image Preprocessing: Images were resized and normalized to optimize YOLOv5 input.
Model Architecture
YOLOv5 was selected for its real-time detection capabilities with the following architecture:

Backbone: CSPDarknet53 for feature extraction.
Neck: PANet layers for feature fusion.
Head: Outputs bounding boxes and class probabilities.
Hyperparameters
Input Size: 416x416 pixels
Batch Size: 16
Epochs: 50
Learning Rate: Experimented with values from 0.001 to 0.01
Results
The model was trained for 25 epochs with the following results:

Validation Accuracy: Approximately 85%
Training Loss: Converged after 25 epochs
Conclusion
This project successfully implemented YOLOv5 for detecting road conditions and turns on Gilgit roads, showing promising results for real-time detection.

Key Achievements
Model Accuracy: Achieved around 85% accuracy on validation.
Data Augmentation: Techniques like rotation and scaling improved model generalization.
Visualization: Result visualizations helped assess detection quality.
Future Work
Increasing Dataset Diversity: Adding more varied samples under different lighting and weather conditions.
Enhanced Model Architecture: Exploring YOLOv8 or hybrid architectures to boost accuracy.
Real-time Application: Deploying the model for real-time inference in autonomous navigation or driver assistance systems.
This README provides an overview of the project objectives, dataset, model architecture, results, and future directions. Make sure to update any specific links or citations if your GitHub repository includes additional resources or documentation.
