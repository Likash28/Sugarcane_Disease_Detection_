###Sugar Cane Disease Detection using ResNet-50 🌿

The **Repo** is a comprehensive exploration of utilizing deep learning for the detection of diseases in sugar cane crops. 🌾

### 🌾 The Problem Statement: Detecting Sugar Cane Diseases

Now, let's remember the quest itself. Our mission is to detect diseases in sugar cane crops. In this age of technology, deep learning is our sword, and the ResNet-50 model is our fortress. By exploring the dataset, preprocessing images, and training our model, we aim to distinguish between healthy and infected sugar cane crops. Our goal is to provide farmers with a tool to protect their valuable crops from diseases. 🌱🛡️

With this code, we embark on a noble journey to safeguard the livelihoods of farmers and ensure the health of sugar cane crops. 🚀🌾🌟

*Let the adventure begin!* 🌟🌿🛡️

#### 📚 Importing Necessary Libraries

The adventure begins with importing some essential libraries. These tools are the sturdy companions that we'll rely on throughout our journey.

- **numpy (np) 🧮**: Our trusty calculator for crunching numbers.
- **pandas (pd) 📊**: Our data librarian for organizing and managing datasets.
- **os 📂**: The guide to navigate the world of files and directories.
- **matplotlib.pyplot 📈**: Our window to visualize data and results.
- **seaborn (sns) 📊**: The artist's palette for making our visualizations more appealing.
- **cv2 (OpenCV) 📷**: The image wizard for image processing tasks.
- **Tensorflow (tf) 🧠**: Our knight in shining armor for building and training deep neural networks.
- **keras. utils.np_utils 🧰**: The tool for working with arrays and encoding labels.
- **keras.models 🏗️**: The architect for constructing neural network models.
- **keras.layers 🧱**: The building blocks for our neural fortresses.
- **TensorFlow. keras.optimizers 🚀**: The captain of the optimization for our models.
- **TensorFlow. keras.layers 🧱**: More building blocks for deep learning structures.

#### 🌄 Exploring the Dataset

Every adventure needs a map, and in our case, it's the dataset. We're on a quest to detect diseases in sugar cane, so we must load the dataset to begin our exploration.

- 🌟 *Data Directory and Class Labels*: We need to establish our destination. In this quest, our sugar cane images will be classified into two categories - "Healthy" and "Infected." These are the class labels guiding our path.

#### 🔍 Data Analysis and Image Processing

Now, it's time for the quest-specific tools to come into play:

- 🕵️ **Error Level Analysis (ELA)**: Think of this as our magnifying glass, helping us detect irregularities in our images. It's used to create an "ELA image" that highlights inconsistencies.

- 🖼️ **Image Preprocessing**: Every explorer needs a trusty assistant, and here we have one! Our assistant, named `prepare_image`, processes each image by converting it to ELA format and resizing it. This step makes the images suitable for our model. 📏

#### 📷 Loading the Adventure Scenes

- Our adventure has two scenes: "Healthy" and "Infected." We load images from both to gather clues for our disease detection mission. 💡

- These images, with their corresponding labels (1 for "Healthy" and 0 for "Infected"), become our companions in this adventure.

#### 🧩 Shuffling and Reshaping

To make the adventure unpredictable, we shuffle the images. Shuffling ensures we don't follow a predictable path and helps in training the model more effectively. The images and labels are shuffled and reshaped for the journey ahead. 🧩

#### 🌟 Splitting the Adventure

An adventure is best when shared, so we split our dataset into two groups - the training party and the validation party. This separation helps us assess our progress more accurately.

#### 🏰 Constructing the ResNet-50 Fortress

The ResNet-50 model is our fortress, designed to protect sugar cane crops from diseases. It's not built from scratch but is adapted from a pre-trained model. We enhance it by adding layers specifically tailored for our disease detection quest. 🏰

#### ⚔️ Preparing for Battle

Our fortress is ready, and it's time for training. We prepare for battle by defining the model's armor and tactics:

- 🛡️ **Categorical Cross-Entropy Loss**: Our compass, guiding us toward the correct path.
- ⚔️ **Adam Optimizer**: The general who leads our troops.
- 🎖️ **Accuracy Metric**: A measure of our success in battle.

We specify the batch size and the number of training epochs, and then the training begins. Our early stopping mechanism ensures we don't overexert ourselves during the journey.

#### 💾 Saving Our Achievements

Every hero needs a memoir. We save the trained fortress (model) as "resnet.h5" to remember our achievements.


