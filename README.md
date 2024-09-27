# Fine-tuned YOLOv8n for Horse Pose Estimation

## Overview
This project extends the YOLOv8 model, trained on the human-centric COCO dataset, to recognize and estimate the poses of horses. Our goal was to test the generalizability of the YOLOv8 pose estimation model by adapting it to a new domain.

## Dataset
The model was trained on the "Horse10" dataset, which comprises annotated images of horses in various poses. This dataset challenges the model with different equine postures not present in typical human pose datasets.

## Model Training
- **Pre-trained Model**: We used the YOLOv8n model pre-trained on the COCO dataset as our starting point.
- **Epochs**: Training was conducted for 50 epochs.
- **Loss Metrics**: Losses tracked include box_loss, pose_loss, obj_loss, cls_loss, and dfl_loss, showing significant convergence by the 40th epoch.

## Performance Metrics
- **Precision and Recall**: Measurements for bounding box (B) and pose (P) estimations were captured, showing substantial improvements and stabilization in the later epochs.
- **mAP Scores**: mAP50 and mAP50-95 scores were calculated to assess model accuracy across different IoU thresholds.
- **F1-Confidence Curve**: Demonstrates the trade-off between precision and recall at various confidence thresholds.

## Results
The model demonstrates high accuracy in recognizing horse features with robust confidence scores for bounding boxes between 0.9 and 1. It shows potential limitations in dynamic keypoints due to the variability in horse movements.

## Usage
To replicate our training or to utilize the fine-tuned model for pose estimation:
1. **Clone the repository**: Access all scripts and training notebooks.
2. **Data**: Download the Horse10 dataset.
3. **Training and Evaluation**: Follow the instructions in the Jupyter notebooks provided.

## Resources
- [Google Drive Link for Project Files](https://drive.google.com/drive/folders/1d9fVKFxu7VuCoVFZafnwSBkWzrkn2_ap?usp=sharing)

## Citation
Please cite this project as follows if you use it for your research:
