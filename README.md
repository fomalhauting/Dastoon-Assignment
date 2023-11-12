# Dastoon-Assignment


## Problem Statement
The goal of this assignment was to develop a deep learning model that can take an existing artwork as inspiration and apply its unique artistic style to a completely new and original piece. Essentially, the model should be capable of analyzing the specific aesthetic characteristics of a chosen artwork and then use this understanding to transform another artwork, making it look like it was crafted by the same artist. In essence, the aim was to create a system that can mimic and adapt artistic styles, producing results that closely resemble the distinctive features of the selected art. This involves the model learning and replicating the intricate details, textures, and overall visual elements that define the chosen artistic style.

## Overview
This repository contains an implementation of Neural Style Transfer using TensorFlow. Neural Style Transfer is an artistic technique that combines the content of one image with the style of another image to create visually appealing and unique artworks.

## Files and Structure
* assignment_dashtoon.ipynb: Jupyter Notebook containing the main code for this Assignment.
* README.md: This document providing an overview of the project and instructions for usage.
* photo.jpg: Sample content image used in the example.
* starry.jpg: Sample style image used in the example.

## Getting Started
1. Clone this repository:
```
git clone https://github.com/your-username/neural-style-transfer.git
cd neural-style-transfer
```
2. Install the required dependencies. Ensure you have TensorFlow and other necessary libraries installed:
```
pip install -r requirements.txt
```
3. Run the neural_style_transfer.ipynb notebook using Jupyter or your preferred Python environment.

## Usage
1. Set the content and style images: Modify the 'content_path' and 'style_path' variables in the notebook to point to your desired content and style images.
```
content_path = 'path/to/your/content/image.jpg'
style_path = 'path/to/your/style/image.jpg'
```
Alternatively, you can use the provided sample images by uncommenting the corresponding lines:
```
content_path = tf.keras.utils.get_file('photo.jpg','https://cera23.iitr.ac.in/wp-content/uploads/2023/03/IITR_JT-1.jpg')
style_path = tf.keras.utils.get_file('starry.jpg','https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcT-YQpREaV8eBEIjkoG3gKa8Q9T_8OvRy4d2z_I7YI-zhjI_7x-')
```
2. Run the notebook cells to perform Neural Style Transfer.

## Customization
Feel free to experiment with the hyperparameters such as 'learning_rate', 'style_weight', 'content_weight', and 'total_variation_weight' to achieve different artistic effects.

### Evaluation Criteria
We can try and assess how accurately the model replicates the artistic style of the reference artwork, by comparing the stylized image with the reference artwork.
This can be achieved by evaluating the similarity in brush strokes, color palette, and overall visual elements.
We can also evaluate the model's ability to retain the key content and structure of the original artwork while applying the new style, by comparing the stylized image with the original artwork.
And focusing on the preservation of objects, shapes, and spatial relationships.
We can also examine the consistency of the applied style throughout the entire stylized image, by analyzing different regions of the image to ensure a coherent application of the chosen artistic style without noticeable inconsistencies.

## Acknowledgments
* This implementation is based on the Neural Style Transfer technique pioneered by Gatys et al. (2015).
* The code uses TensorFlow, an open-source machine learning library.

## Author
Kriti (kriti13kriti@gmail.com)

## Troubleshooting
If you encounter any issues or have questions, please create an issue in the GitHub repository. We'll be happy to assist you.
