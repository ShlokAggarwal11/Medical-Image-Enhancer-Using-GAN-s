# Medical-Image-Enhancer-Using-GAN-s

This repository contains code for a Medical Image Enhancer using Generative Adversarial Networks (GANs) to improve the resolution of medical images. The code uses TensorFlow and TensorFlow Hub to load a pre-trained GAN model for super-resolution.

## Installation

Before running the code, make sure you have the required dependencies installed. You can install them using the following command:

```bash
pip install -q gwpy
```

## Usage

1. Clone the repository to your local machine.

2. Install the required packages by running the installation command mentioned above.

3. Download the pre-trained GAN model by running the following command:

```bash
SAVED_MODEL_PATH="https://tfhub.dev/captain-pool/esrgan-tf2/1"
```

4. Load the pre-trained model and preprocess the medical image for enhancement by providing the path to the medical image in the `IMAGE_PATH` variable:

```python
IMAGE_PATH = "path_to_your_medical_image.jpg"
```

5. Execute the code to perform super-resolution on the medical image:

```bash
python medical_image_enhancer.py
```

The script will preprocess the medical image, perform super-resolution using the GAN model, and display the enhanced image. It will also calculate the Peak Signal-to-Noise Ratio (PSNR) achieved by the enhancement.

## Output

The output will include the enhanced medical image along with the PSNR achieved compared to the original image.

## Note

Please ensure that you have a compatible version of TensorFlow and TensorFlow Hub installed before running the code. Additionally, make sure you have the necessary permissions to download the pre-trained GAN model.

## Disclaimer

This code is for educational and research purposes only. It is not intended for medical diagnosis or treatment. Please consult a qualified medical professional for medical advice.

Feel free to reach out if you have any questions or feedback! Happy image enhancement!
