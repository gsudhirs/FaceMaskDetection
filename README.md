# FaceMaskDetection
A convolutional neural network model with the capability of discerning whether a given face is wearing a mask or not.

![image](https://user-images.githubusercontent.com/111015445/219254097-32101f77-1280-48e2-99d7-12a6c257f18b.png)

The face detection model and the face mask classification are used together to detect whether multiple faces in a given frame are wearing a mask or not wearing a mask. The face detection model returns a list of values representing the bounding boxes coordinates around the detected faces. Using these coordinates, the detected face is cropped and resized into 100 by 100. The resultant image is used as an input to the face mask classification model. Based on the prediction made by the face mask classification model, the color of bounding box around the detected face changes. If the face mask is detected, then the color of bounding box is green, else the color of bounding box is red.

Inspired by the following paper:

S. Abbasi, H. Abdi and A. Ahmadi, "A Face-Mask Detection Approach based on YOLO Applied for a New Collected Dataset," 2021 26th International Computer Conference, Computer Society of Iran (CSICC), Tehran, Iran, 2021, pp. 1-6, doi: 10.1109/CSICC52343.2021.9420599.

Dataset taken from:
https://www.kaggle.com/datasets/ashishjangra27/face-mask-12k-images-dataset
https://www.kaggle.com/datasets/prasoonkottarathil/face-mask-lite-dataset
