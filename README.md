# Damalerio-Nikko_LW1_Image_Classification

🔗 **Google Colab Notebook:**  
[Click here to open in Google Colab](https://colab.research.google.com/drive/1PBgdii8UpFXVC9-8a4TfrOeYw2N0EWiZ?usp=sharing)

---

## Questions and Answers

### 1. What is the Fashion MNIST dataset?

**Answer:**  
The Fashion MNIST dataset is a pre-made dataset that contains grayscale images of clothing and accessories. Each image is 28×28 pixels, and the dataset is divided into training and testing sets. It includes 10 different categories such as:

- T-shirt/top  
- Trouser  
- Pullover  
- Dress  
- Coat  
- Sandal  
- Shirt  
- Sneaker  
- Bag  
- Ankle boot  

Unlike the original MNIST dataset, which uses handwritten digits (0–9), Fashion MNIST is used to classify fashion items.

---

### 2. Why do we normalize image pixel values before training?

**Answer:**  
Image normalization is done to make training faster and more stable for the neural network. Original pixel values range from 0 to 255, and large values can slow down learning and make optimization harder. By dividing the pixel values by 255, we scale them to a range between 0 and 1. This keeps the image information the same while allowing the model to learn more efficiently.

---

### 3. List the layers used in the neural network and their functions.

**Answer:**  
The neural network used in this model has three layers:

- **Flatten layer:**  
  Converts each 28×28 image into a one-dimensional array of 784 values so it can be processed by the dense layers.

- **Dense hidden layer (ReLU):**  
  Contains 128 neurons and uses the ReLU activation function. It helps the model learn important patterns and features from the images, such as shapes and edges.

- **Output Dense layer:**  
  Has 10 neurons, one for each clothing category. It outputs scores for each class, and the highest score determines the predicted label.

---

### 4. What does an epoch mean in model training?

**Answer:**  
An epoch represents one complete pass of the entire training dataset through the neural network. Increasing the number of epochs allows the model to learn more from the data, but too many epochs can cause overfitting.

---

### 5. Compare the predicted label and actual label for the first test image.

**Answer:**  
For the first test image, the model predicted the label as **9**, which corresponds to **Ankle boot**. The actual label is also **9 (Ankle boot)**. This means the model correctly classified the image.

---

### 6. What could be done to improve the model’s accuracy?

**Answer:**  
The model’s accuracy can be improved in several ways, such as:

- Adding more hidden layers to learn more complex patterns  
- Increasing the number of neurons or changing activation functions  
- Training the model for more epochs  
- Using techniques like dropout or convolutional layers  

These improvements can help the model generalize better and achieve higher accuracy.
