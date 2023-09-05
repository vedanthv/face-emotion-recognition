# Unveiling Emotions: Decoding Sentiments through Textual Analysis

In this project, we extensively focus on leveraging texture-based facial feature representations of the eyes, ears, and nose through image processing and custom feature extraction techniques on existing datasets to enhance evaluation metrics, addressing various applications like video surveillance and anti-spoof detection in Facial Emotion Recognition (FER).
## Datasets
1. **FER-2013**:The data consists of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centred and occupies about the same amount of space in each image.The task is to categorize each face based on the emotion shown in the facial expression into one of seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral). The training set consists of 28,709 examples and the public test set consists of 3,589 examples.

## Description of the project

Our project represents a significant advancement in the field of Facial Emotion Recognition (FER) by focusing on a texture-based approach that leverages facial features such as the eyes, ears, and nose. While FER has been a prominent area of research for years, traditional methods often struggled to capture the nuanced emotional subtleties in facial expressions. We recognized the limitations of existing techniques, which relied on geometric features or appearance-based methods and often required extensive data and computational resources, leading to lower accuracy.

In response, our project delves into the intricate texture patterns of the face, including wrinkles, skin texture, furrows, and micro-movements. These subtle details can be crucial in expressing emotions, as expressions like happiness or surprise can be indicated by slight changes in the skin around the eyes or the appearance of fine lines on the forehead. By harnessing these valuable insights from diverse texture patterns across facial regions, our approach offers a more profound and comprehensive understanding of distinct emotional states.

One of the key advantages of our texture-based approach is its robustness. Factors such as changes in lighting, variations in pose, and the presence of obstructions like glasses or facial hair often challenge traditional FER methods. However, texture-based analysis is less susceptible to these influences. Even in challenging conditions like low lighting, the texture of the face remains relatively stable, providing reliable information about emotions. This resilience makes texture-based approaches highly adaptable and ensures dependable recognition in diverse real-life contexts.

In our project, we have invested significant effort in implementing image processing algorithms and custom feature extraction techniques on existing datasets. Through rigorous experimentation, we have demonstrated how our approach improves evaluation metrics, showcasing its potential applications in various domains. Specifically, we have highlighted its usefulness in video surveillance, where recognizing emotions can enhance security and situational awareness, as well as in anti-spoof detection, where distinguishing real faces from fake ones is crucial for authentication and security purposes. Our work represents a pioneering step towards more accurate and adaptable Facial Emotion Recognition, with wide-ranging implications for both academic research and commercial applications.

## Getting Started

### Dependencies

1. **Operating System**: The project is platform-independent and can be run on various operating systems, including Windows 10, macOS, and Linux distributions.

2. **Programming Language**: The project is implemented using programming language Python

3. **Python Version**: The project requires Python 3.x, and it's recommended to use the latest stable version available at the time of installation.

4. **Libraries**:
   - **OpenCV**: OpenCV is essential for image processing and computer vision tasks. Version 4.x or later is recommended.
   - **NumPy**: NumPy is used for numerical operations and array manipulation in Python.
   - **TensorFlow or PyTorch**: Depending on the deep learning framework chosen for implementing the neural network models. Either TensorFlow or PyTorch should be installed.
   - **Scikit-learn**: If machine learning algorithms are used alongside deep learning techniques, Scikit-learn is helpful for data preprocessing and evaluation.
   - **Matplotlib**: Matplotlib is used for data visualization and plotting graphs to visualize project results.
   - **Pandas**: Pandas is used for data manipulation and analysis.
   
5. **GPU Support** (Optional): If you intend to accelerate deep learning model training, having a compatible NVIDIA GPU and installing CUDA and cuDNN libraries might be necessary for TensorFlow or PyTorch, depending on your choice.

6. **Dataset**: Depending on the specific datasets used for training and testing the models, you should have access to and permissions to use the relevant facial emotion recognition datasets.

7. **Development Environment**: An integrated development environment (IDE) like Jupyter Notebook or a code editor like Visual Studio Code can be helpful for code development and experimentation.

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

1. Vedanth Baliga
2. Yashna Karkera
3. Abhiruchi Bharambe
4. Nandini Hazarika

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
