### Proposed Techniques

### ****************************Preprocessing****************************

1. ************************************************Face Alignment Detectors************************************************
    - **Viola-Jones face detector** - removes background and focuses on face only
    - **Active Appearance Model** - Generative Model
    - **Mixture of Trees and Discriminative Response Map Filtering** - Localized feature detection
    - ****************************************************************************Supervised Descent Method -**************************************************************************** regressive function that maps images to localized facial landmarks
    - **Task Constrained Deep Neural Network and Cascaded CNN** - SOTA models for face alignment
2. **********************************Data Augmentation**********************************
    - **Randomly crop images** from 4 corners and flip them
    - **Use only center patch** facial textures in the dataset
    - **Rotation, Shifting, Skew and Contrast General Methods**
    - **Salt and Pepper Noise, Spekle Noise and Gaussian Noise**
    - **3D Convolutional Neural Network** to create a synthetic dataset with different levels of saturation
3. ************************Face Normalization************************
    1. **********Illumination Normalization********** 
        - ****************Isotropic Diffusion**************** Based Normalization
        - ********************************************Discrete Cosine Transforms******************************************** Based Normalization
        - **********Homomorphic Filter********** based Normalization
        - ********************************Histogram Equalization -******************************** improves global contrast
        - ************************************************Weighted Sum Approach************************************************ of Histogram Equalization and Linear Mapping
        - ********************************************Global Contrast Normalization -******************************************** SOTA
    2. ************************************Pose Normalization************************************
        - Face Normalization[localize texture landmarks on face] + mask on 3D reference model of face.
        - FF-GAN, TP-GAN, DR-GAN

### Implented Techniques

| Dataset | Technique | Research Paper  | Description   |
| ------ |----------|-------------------| ------------ |
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Blur and Rotate](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/blur-and-rotate.ipynb)|NA|Blur the image and rotate it in 3 ways|
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Gaussian Unsharp Mask](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/unsharping.ipynb)|NA|Tuning of Sigma Parameter of Gaussian Model and Scaling Factor to control sharpness|
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Edge Detection](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/edge-detection.ipynb)|NA|Examines an image and identifies the edges and boundaries present within it|
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Denoising](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/notebookname.ipynb)|NA|Removes or reduces the unwanted noise from an image while preserving the important details and features|
