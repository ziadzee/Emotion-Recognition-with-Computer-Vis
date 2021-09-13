# Emotion Recognition using Computer Vision

- Implemented different computer vision techniques in order to detect emotion in images and videos. Utilised `SVM`, `MLP` and `CNN` models. 

- For the `SVM` and `MLP` I also implemented three detection methods: `Histograms of Oriented Gradients (HOG)`,  `Scale-Invariant Feature Transform (SIFT)` and `Oriented FAST and rotated BRIEF (ORB)` to compare performance.

- Used Grid Search for `SVM` and `MLP` for hyperparameter tuning. 

- Implemented custom test functions to load and predict images and videos.


# Packages
- Python Version: `3.8.11`

- Libraries and Packages: `numpy` , `pandas`, `seaborn`, `torch`, `torchvision`, `PIL`, `cv2` , `sklearn` , `skimage`

# Outcomes
### Detector Methods:

- Best performing detection method is HOG across both the MLP and SVM models which achevied F1 scores of 0.64 and 0.65 respectively:

![image](https://user-images.githubusercontent.com/65977822/133061002-5714e3a6-7ca9-491c-a31e-b2a2c78c512e.png)

ORB: 

![image](https://user-images.githubusercontent.com/65977822/133061264-e7e8dc94-f7d9-477a-bbf1-ba1d1287bb6b.png)

SIFT:

![image](https://user-images.githubusercontent.com/65977822/133061516-bdaade82-5b9e-4507-9286-bd15331238a9.png)

HOG:

![image](https://user-images.githubusercontent.com/65977822/133061603-8919923a-3450-4f66-8f64-de61ed3d6f3c.png)

![image](https://user-images.githubusercontent.com/65977822/133061799-798660a9-a9ae-4f8e-b925-710c20991ac8.png)
![image](https://user-images.githubusercontent.com/65977822/133061876-fa68f4ae-d108-434c-a0ed-e52801bd626a.png)
![image](https://user-images.githubusercontent.com/65977822/133061907-b2649d77-17e2-4cbb-b309-6a6c4d06bd7d.png)

### Convolutional Neural Networks:

- I tried several different CNN architectures including: `AlexNet`, `VGG16`, `GoogLeNet` `ResNetXt and a vanilla `MLP`. The best performing CNN was `VGG16` which achieved an accuracy score of 0.81 after 5500 iterations. When testing, it was observed that the `VGG16` model was incorrect in some instances and failed to adequately detect emotions on multiple faces in a given frame.

![image](https://user-images.githubusercontent.com/65977822/133062257-f0a47c61-4af0-4255-8fe2-3ff46d2a1a59.png)

# Specifications

Code, data and files for the above can be found in the following files:

- `CNN`, `MLP`, `SVM`: code for all models and outcomes 
- `Dataset`: the image data used to train all models. Note: for copyright reasons the images are not included in this repo
- `Test_Functions`: contains the code for the test functions used for all models
- `Videos`: test videos for CNN
