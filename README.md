# Black and White Image Colorization with OpenCV and Deep Learning

## Overview
This project focuses on colorizing black and white images using deep learning techniques with OpenCV. A pre-trained deep neural network is utilized to add realistic colors to grayscale images.

## Dataset
The dataset consists of grayscale images that are colorized using a deep learning model trained on large-scale datasets like:
- ImageNet
- Places365

## Model Architecture
This project uses a deep learning model trained on colorization tasks, such as:
- **DeOldify**
- **Caffe-based Colorization Model**
- **U-Net based architectures**

## Installation and Dependencies
To run this project, install the necessary dependencies:
```bash
pip install opencv-python numpy matplotlib tensorflow
```

## Implementation Steps
1. Load a pre-trained colorization model.
2. Convert the input image to the LAB color space.
3. Extract the L channel (grayscale) and feed it into the model.
4. Obtain the predicted A and B channels.
5. Merge the predicted A and B channels with the original L channel.
6. Convert back to the RGB color space and display the output.

## Usage
- Run the colorization script:
```bash
python colorize.py --image path/to/grayscale_image.jpg
```

## Results
The model generates realistic colorized versions of black and white images. Evaluation metrics include:
- Structural Similarity Index (SSIM)
- Peak Signal-to-Noise Ratio (PSNR)

## Future Improvements
- Improve model accuracy with more training data
- Implement real-time video colorization
- Optimize inference speed for better performance

## Acknowledgments
- OpenCV for image processing
- Deep learning research in colorization techniques

## License
This project is open-source and available under the MIT License.

