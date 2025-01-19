![IEEE Published](https://img.shields.io/badge/Published%20on-IEEE-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Python](https://img.shields.io/badge/Python-3.7%2B-yellow)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen)


# American Sign Language Detection using TensorFlow

Developed a sign language detection system using advanced technologies including machine learning and TensorFlow (Object Detection API).

---

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Prerequisites](#prerequisites)
5. [Installation](#installation)
6. [Dataset](#dataset)
7. [Usage](#usage)
8. [Results](#results)
9. [Future Enhancements](#future-enhancements)
10. [Contributing](#contributing)
11. [License](#license)

---

## Introduction
This project implements a system to detect and interpret American Sign Language (ASL) using machine learning models. The goal is to bridge communication gaps and provide a practical solution for individuals with hearing or speech impairments.

---

## Publication
This project was presented and published at the **[ACDSA IEEE International Conference on Artificial Intelligence, Computer, Data Sciences and Applications](https://www.acdsa.org)**.  
- **Paper Title**: [Real Time Sign Language Detection](https://ieeexplore.ieee.org/document/10467736/authors#authors)  
- **DOI**: [DOI Link](link-to-doi)
- **Conference Details**: [2024 International Conference on Artificial Intelligence, Computer, Data Sciences and Applications (ACDSA)](https://www.acdsa.org)

---

## Citation
S. Swaroop, K. Y. Prasad, G. Sai Srikar Reddy, M. Rachavelpula and U. A. Jogalekar, "Real Time Sign Language Detection," 2024 International Conference on Artificial Intelligence, Computer, Data Sciences and Applications (ACDSA), Victoria, Seychelles, 2024, pp. 1-7, doi: 10.1109/ACDSA59508.2024.10467736. keywords: {Training;Deep learning;Sign language;Computer vision;Adaptation models;Pipelines;Computer architecture;Sign Language Detection;OpenCV;LabelImg;Tensorflow;Pipeline Deep Learning;Communication Technology;Accessibility;Inclusivity;Computer Vision;Dataset Curation;Neural Networks;Communication Barriers;Assistive Technology;Language Interpretation},

---

## Features
- Real-time sign language detection and interpretation.
- Highly accurate recognition using TensorFlow’s Object Detection API.
- Easy-to-use interface with support for multiple signs.
- Extensible and customizable for additional sign languages.

---

## Technologies Used
- **Python**: Programming language for implementing the detection system.
- **TensorFlow**: For building and training machine learning models.
- **OpenCV**: For image processing and real-time video stream handling.
- **Jupyter Notebook**: For experimentation and visualization.

---

## Prerequisites
Ensure the following tools and libraries are installed:
- Python 3.7 or later
- OpenCV
- TensorFlow
- Jupyter Notebook

---

## Installation
Follow these steps to set up the project:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AmericanSignLanguageDetection-TF.git
   cd AmericanSignLanguageDetection-TF
   ```
2. Create a virtual environment:
   ```bash
   python -m venv asl_env
   source asl_env/bin/activate  # On Windows: asl_env\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up TensorFlow Object Detection API (follow [official guide](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/)).

---

## Dataset
The system uses a labeled dataset of ASL gestures. You can:
1. Use an existing dataset (e.g., [ASL Alphabet Dataset](https://www.kaggle.com/grassknoted/asl-alphabet)).
2. Create a custom dataset by capturing images of gestures.

For training, ensure the dataset is annotated in a format compatible with TensorFlow’s Object Detection API (e.g., TFRecord).

---

## Usage
1. Train the model:
   - Update the `pipeline.config` file with dataset paths and training parameters.
   - Run the training script:
     ```bash
     python model_main_tf2.py --model_dir=models/ --pipeline_config_path=models/pipeline.config
     ```
2. Evaluate the model:
   ```bash
   python model_main_tf2.py --model_dir=models/ --pipeline_config_path=models/pipeline.config --checkpoint_dir=models/
   ```
3. Run real-time detection:
   ```bash
   python detect_signs.py
   ```

---

## Results
- Achieved an accuracy of XX% on the validation dataset.
- Demonstrated robust performance in real-time detection scenarios.

---

## Future Enhancements
- Expand support for additional sign languages.
- Integrate with wearable devices for seamless communication.
- Improve detection accuracy with larger datasets and advanced architectures.

---

## Contributing
Contributions are welcome! Follow these steps to contribute:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## License
This project is licensed under the [MIT License](LICENSE).

