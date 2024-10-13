# Mole Classification Model

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/lorenzopalaia/mole-classification">
    <img src="repo_assets/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Mole Classification Model</h3>

  <p align="center">
    A deep learning model to classify moles as benign or malignant based on images.
    <br />
    <a href="https://github.com/yourusername/mole-classification"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/yourusername/mole-classification">View Demo</a>
    ·
    <a href="https://github.com/yourusername/mole-classification/issues">Report Bug</a>
    ·
    <a href="https://github.com/yourusername/mole-classification/issues">Request Feature</a>
  </p>
</div>

## About The Project

This project develops a convolutional neural network (CNN) model to classify moles as either benign or malignant based on dermatoscopic images. It provides an accessible and efficient way to assist in the early detection of skin cancer.

The project includes the following steps:

1. **Data Preprocessing**: Images are preprocessed by resizing, normalizing, and converting them into an array suitable for input into the model.

2. **Model Development**: The model uses a deep learning architecture built with Keras in TensorFlow, designed to classify images into two categories: benign and malignant.

3. **Model Evaluation**: After training, the model's performance is evaluated using accuracy and confidence metrics. The results provide insights into the reliability of the model in identifying skin lesions.

4. **Usage & Deployment**: The final model is ready to be integrated into applications that can assist medical professionals in diagnosing skin conditions based on images.

### Built With

- Python
- TensorFlow / Keras
- Numpy
- PIL (Python Imaging Library)
- Matplotlib

## Getting Started

To get a local copy of the project up and running, follow these simple steps.

### Prerequisites

- Python 3.x
- Pip (Python package installer)

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/lorenzopalaia/mole-classification.git
   ```
2. Navigate to the project directory:
   ```
   cd mole-classification
   ```
3. Install the required Python packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

You can run the model on your local machine to classify moles based on images. The project provides Python scripts for preprocessing images and making predictions. Follow the steps below to load an image and get the classification results:

```python
# Example code snippet from the notebooks
from PIL import Image
import matplotlib.pyplot as plt

# Load and display the mole image
img_path = "/data/my_mole.jpg"
img = Image.open(img_path)
plt.imshow(img)
plt.axis('off')
plt.show()

# Make a prediction
predicted_class, confidence = make_prediction(img_path)
print(f"Predicted class: {predicted_class}, Confidence: {round(confidence * 100, 2)}%")

# Perform additional analysis or model fine-tuning
# ...
```

For more detailed usage examples and instructions, please refer to the [Documentation](https://github.com/lorenzopalaia/mole-classification).

## Roadmap

- [ ] Explore additional skin condition classifications
- [ ] Improve model accuracy with more advanced architectures
- [ ] Deploy the model as a web service or mobile app for real-time usage
- [ ] Expand the dataset for more diverse training

See the [open issues](https://github.com/lorenzopalaia/mole-classification/issues) for a full list of proposed features (and known issues).

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

## Contact

Lorenzo Palaia - lorenzopalaia53@gmail.com

Project Link: [https://github.com/lorenzopalaia/mole-classification](https://github.com/lorenzopalaia/mole-classification)

[contributors-shield]: https://img.shields.io/github/contributors/lorenzopalaia/mole-classification.svg?style=for-the-badge
[contributors-url]: https://github.com/lorenzopalaia/mole-classification/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/lorenzopalaia/mole-classification.svg?style=for-the-badge
[forks-url]: https://github.com/lorenzopalaia/mole-classification/network/members
[stars-shield]: https://img.shields.io/github/stars/lorenzopalaia/mole-classification.svg?style=for-the-badge
[stars-url]: https://github.com/lorenzopalaia/mole-classification/stargazers
[issues-shield]: https://img.shields.io/github/issues/lorenzopalaia/mole-classification.svg?style=for-the-badge
[issues-url]: https://github.com/lorenzopalaia/mole-classification/issues
[license-shield]: https://img.shields.io/github/license/lorenzopalaia/mole-classification.svg?style=for-the-badge
[license-url]: https://github.com/lorenzopalaia/mole-classification/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/lorenzopalaia
