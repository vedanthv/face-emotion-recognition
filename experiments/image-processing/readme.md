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
      
### Models for Facial Emotion Recognition

1. **Convolutional Neural Networks**
- Used a blend of cutting edge learnable filters on the images to convolve and produce unique feature maps and embeddings that are then pooled to reduce the dimensionality.
- Some common models that have been used on a mixture of more than 5 datasets are:
      - ResNet50 and ResNet 128
      - Region Based CNN(RCNN) and Fast-RCNN
      - Motion Capture and Frame By Frame Sequential 3D CNN

2. **Deep Autoencoders**
- DAEs are implemented to preserve the context and quality of images after dimensionality reduction.
- Fine Tuned Denoising Auto Encoder models used to reconstruct images that have noise embedded in them.
- Variational Auto Encoders and Decoders used to modify DAE by using Graphical Networks.
- Stacked Convolutional Auto Encoders used to denoise images without dimensionality reduction using filters and optimized pooling layers.

3. **Recurrent Neural Networks**
- Modification of the popular RNN with input, output and forget gates to include a accumulation gate that can identify crucial features in the image with less number of filtering layers and can capture sequential image data, remembering the context information and change in emotions also. Some variations like GRU and LSTM are also tested on a custom dataset with 3-4 benchmarking datasets.

4. **Generative Adversial Networks**
- We aim to create a model to control the information output of the discriminator using certain conditions and filters that were utilized in the preprocessing stage. Some GAN models that can be utilized are DGCNN networks that is a blend of 2 CNN models for disriminator and generator networks and finally their outputs can be compared. Other type of GAN is VAEGAN that uses the discriminator to learn features from the images and generator that uses VAE to reconstruct the images.

### Implented Techniques

| Dataset | Technique | Research Paper  | Description   |
| ------ |----------|-------------------| ------------ |
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Blur and Rotate](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/blur-and-rotate.ipynb)|NA|Blur the image and rotate it in 3 ways|
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Gaussian Unsharp Mask](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/unsharping.ipynb)|NA|Tuning of Sigma Parameter of Gaussian Model and Scaling Factor to control sharpness|
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Edge Detection](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/edge-detection.ipynb)|NA|Examines an image and identifies the edges and boundaries present within it|
|[Kaggle FER](https://www.kaggle.com/datasets/msambare/fer2013)|[Denoising](https://github.com/vedanthv/face-emotion-recognition/blob/main/experiments/image-processing/notebookname.ipynb)|NA|Removes or reduces the unwanted noise from an image while preserving the important details and features|
