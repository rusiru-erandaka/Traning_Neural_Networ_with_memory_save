# 🧠 CNN Training: Standard vs Memory-Efficient Approaches

This repository explores two distinct methods of training Convolutional Neural Networks (CNNs) for image classification:

- **Standard Approach**: Loading the dataset into memory.
- **Memory-Efficient Approach**: Streaming images directly from URLs to conserve RAM usage.

By comparing these workflows, this project provides insight into practical deep learning on machines with limited memory resources.

---

## 📁 Project Structure

```bash
📦CNN-Training-Memory-Efficient
 ┣ 📓 CNN_training.ipynb
 ┣ 📓 CNN_training_memory_save.ipynb
 ┣ 📓 Data_preprocessing.ipynb
 ┗ 📓 Data_preprocessing_memory_save.ipynb

```
<br>

## 🚀 Key Features

- ✅ CNN implementation using TensorFlow/Keras
- ✅ Efficient memory-saving techniques (image streaming)
- ✅ Dataset preprocessing with and without memory constraints
- ✅ Training and evaluation pipeline
- ✅ Clear performance comparison (speed, RAM usage, accuracy)

<br>

## 🧪 Notebooks Overview

### 📓 Data_preprocessing.ipynb
- Loads image data into memory.
- Applies transformations like resizing, normalization, and label encoding.
- Prepares NumPy arrays for model input.

### 📓 Data_preprocessing_memory_save.ipynb
- Skips loading all images into RAM.
- Uses image URLs with on-the-fly processing via PIL and TensorFlow's tf.data.
- Ideal for handling large datasets or running on low-memory machines.

### 📓 CNN_training.ipynb
- Trains a CNN on preprocessed in-memory data.
- Uses Keras Sequential API.
- Includes model evaluation and accuracy tracking.

<br>

## 📦 Installation

```bash
git clone https://github.com/rusiru-erandaka/Traning_Neural_Networ_with_memory_save.git
cd Traning_Neural_Networ_with_memory_save
```

## 📊 Example Usage

Run standard training:

```bash
jupyter notebook CNN_training.ipynb
```
Run memory-efficient training:

```bash
jupyter notebook CNN_training_memory_save.ipynb
```

## 🧠 Insights & Comparisons

| **Aspect**      | **Standard Method**            | **Memory-Saving Method**          |
|-----------------|--------------------------------|-----------------------------------|
| **RAM Usage**   | High                           | Low                               |
| **Speed**       | Faster (with enough RAM)       | Slower (due to image streaming)   |
| **Suitability** | High-end machines              | Low-resource environments         |
| **Accuracy**    | Comparable                     | Comparable                        |


## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to fork the repo and submit a pull request.


