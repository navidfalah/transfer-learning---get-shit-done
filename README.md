# Traffic Sign Classification with Transfer Learning 🚦🤖

This project demonstrates **transfer learning** using a pre-trained **ResNet34** model to classify traffic signs. The goal is to classify traffic signs into categories such as "priority road," "give way," "stop," and "no entry," while also handling unknown signs. 🎯📊

---

## Table of Contents 📑
1. [Overview](#overview-)
2. [Installation](#installation-)
3. [Usage](#usage-)
4. [Code Structure](#code-structure-)
5. [Results](#results-)
6. [License](#license-)

---

## Overview 🚀

This project:
- Uses **transfer learning** with a pre-trained ResNet34 model for traffic sign classification. 🤖📸
- Handles **unknown traffic signs** by adding an "unknown" class to the dataset. 🧠🔍
- Implements data augmentation, model training, and evaluation. 📊📉

---

## Installation 🛠️

To run this project, you need to install the required libraries. Run the following commands:

```bash
!pip install torch torchvision pandas numpy matplotlib seaborn tqdm scikit-learn
```

---

## Usage 🖥️

1. **Load Dataset**: The script downloads and loads the GTSRB (German Traffic Sign Recognition Benchmark) dataset.
2. **Preprocess Data**: Applies data augmentation, normalization, and splits the data into training, validation, and test sets.
3. **Build Model**: Defines and trains a ResNet34 model using transfer learning.
4. **Evaluate Model**: Evaluates the model's performance on test data and visualizes results.
5. **Handle Unknown Signs**: Adds an "unknown" class to handle unseen traffic signs.

---

## Code Structure 🗂️

- **Data Preparation**:
  - Downloads and preprocesses the GTSRB dataset.
  - Splits the data into training, validation, and test sets.

- **Model Definition**:
  - Uses a pre-trained ResNet34 model for transfer learning.
  - Adds a custom classification head for traffic sign classification.

- **Training**:
  - Trains the model using the training set.
  - Tracks training and validation accuracy and loss.

- **Evaluation**:
  - Evaluates the model's performance on the test set.
  - Visualizes predictions, confusion matrices, and classification reports.

- **Handling Unknown Signs**:
  - Adds an "unknown" class to the dataset.
  - Retrains the model to handle unknown traffic signs.

---

## Results 📊

- **Training/Validation Accuracy**: The model achieves high accuracy on the training and validation sets.
- **Test Accuracy**: Evaluates the model's performance on the test set.
- **Unknown Sign Handling**: Demonstrates the model's ability to classify unknown traffic signs.

---

## License 📜

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it as needed.

---

## Example Output 🖼️

Here’s an example of the model's training progress:

```plaintext
Epoch 1/10: train loss: 0.123, train acc: 0.987, valid loss: 0.045, valid acc: 0.991
Epoch 2/10: train loss: 0.045, train acc: 0.991, valid loss: 0.032, valid acc: 0.993
```

---

## Dependencies 📦

- `torch`
- `torchvision`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `tqdm`
- `scikit-learn`

---

## Author 👨‍💻

This project was created by **[Navid Falah](https://github.com/navidfalah)**. Feel free to reach out for questions or collaborations at **navid.falah7@gmail.com**! 🤝
