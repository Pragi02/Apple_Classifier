# Yolov7 Object detection 

YOLOv7 surpasses all known object detectors in both speed and accuracy in the range from 5 FPS to 160 FPS and has the highest accuracy 56.8% AP among all known real-time object detectors with 30 FPS or higher on GPU V100. YOLOv7-E6 object detector (56 FPS V100, 55.9% AP) outperforms both transformer-based detector SWIN-L Cascade-Mask R-CNN (9.2 FPS A100, 53.9% AP) by 509% in speed and 2% in accuracy, and convolutional-based detector ConvNeXt-XL Cascade-Mask R-CNN (8.6 FPS A100, 55.2% AP) by 551% in speed and 0.7% AP in accuracy, as well as YOLOv7 outperforms: YOLOR, YOLOX, Scaled-YOLOv4, YOLOv5, DETR, Deformable DETR, DINO-5scale-R50, ViT-Adapter-B and many other object detectors in speed and accuracy. Moreover, we train YOLOv7 only on MS COCO dataset from scratch without using any other datasets or pre-trained weights. 

### Dataset : Apple classification between ripe and unripe

Model Architecture : Extended efficient layer aggregation networks (E-ELAN)YOLOv7 Architecture Extended Efficient Layer Aggregation Network (E-ELAN)
Model Scaling for Concatenation based Models 
Trainable Bag of Freebies Planned re-parameterized convolution 
Coarse for auxiliary and fine for lead loss  

### Classes:
 1. Ripe apple
 2. Unripe apple


### F1 Curve
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/F1_curve.png)

### Precision Curve
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/P_curve.png)

### Recall Curve
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/R_curve.png)

### Precision Recall Curve
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/PR_curve.png)

### Confusion Matrix
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/confusion_matrix.png)

## Prediction 
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/test_batch0_pred.jpg)

## Labels
![alt text](https://github.com/Pragi02/Apple_Classifier/blob/main/test_batch0_labels.jpg)

## Results: 
1. box_loss — bounding box regression loss (Mean Squared Error).
2. obj_loss — the confidence of object presence is the objectness loss (Binary Cross Entropy).
3. cls_loss — the classification loss (Cross Entropy).
4. Precision measures how much of the bbox predictions are correct ( True positives / (True positives + False positives)), 
5. Recall measures how much of the true bbox were correctly predicted ( True positives / (True positives + False negatives)). 
6. ‘mAP_0.5’ is the mean Average Precision (mAP) at IoU (Intersection over Union) threshold of 0.5.
7. ‘ mAP_0.5:0.95’ is the average mAP over different IoU thresholds, ranging from 0.5 to 0.95.
