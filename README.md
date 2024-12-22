# Facial Image Generation using GANs

## Project Overview
This project demonstrates the implementation of a Face Generation algorithm using Generative Adversarial Networks (GANs). The goal of the project is to create a facial image generation model that can generate new facial images based on a dataset and text prompts.

## Dataset
The dataset for this project was constructed by students enrolled in the Deep Learning course. It contains facial images collected as follows:

- **Total images**: 40 facial images per student
- **Image format**: JPEG
- **Resolution**: At least 500 × 500 pixels
- **Subjects**: Individuals facing the front with a neutral expression
- **Image content**: Solo images with no other objects or special lighting
- **Face coverage**: Large part of the image is the face
- **Additional collected details**: 
  - Type of Lip
  - Colour of Lip
  - Forehead
  - Cheeks with dimple
  - Ear
  - Eye Size
  - Eye Defect
  - Eye Color
  - Eyebrow style
  - Jaw Line
  - Skin Color
  - Hair Colour
  - Hair Style
  - Beard/Mustache
  - Age
  - Gender
  - Identification Mark

This dataset serves as the input for the GAN model.

## GAN Model Architecture
The project utilizes a **Generative Adversarial Network (GAN)**, which consists of two neural networks: the generator and the discriminator. 

- **Generator**: Generates synthetic data that mimics the distribution of the dataset.
- **Discriminator**: Differentiates between real and fake data.

The GAN operates by engaging the generator and discriminator in an adversarial process, where:
- The generator creates fake samples.
- The discriminator tries to classify samples as real or fake.

### Architecture Details:
- Both the generator and discriminator consist of 5 hidden layers.
- **Activation functions**:
  - Discriminator hidden layers: Leaky ReLU
  - Discriminator output layer: Sigmoid
  - Generator hidden layers: ReLU
  - Generator output layer: Tanh

## Results
The following table shows the performance of the GAN at different epochs.

| Epoch | Generator Loss | Discriminator Loss | Real Score | Fake Score |
|-------|----------------|---------------------|------------|------------|
| 10    | 3.9590         | 0.3992              | 0.7500     | 0.0036     |
| 20    | 4.5243         | 0.4415              | 0.9007     | 0.2403     |
| 30    | 3.4821         | 0.4104              | 0.7976     | 0.1325     |
| 40    | 2.6479         | 0.4776              | 0.8646     | 0.2552     |

These results show the progress of the GAN model in generating realistic facial images over the epochs.
<img width="758" alt="Screenshot 2024-12-22 at 1 54 10 PM" src="https://github.com/user-attachments/assets/45eeefe8-fa41-4758-b7c8-e188b16dc0f3" />

