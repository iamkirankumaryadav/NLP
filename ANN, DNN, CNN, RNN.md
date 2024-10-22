# ANN | DNN | CNN | RNN

### ANN (Artificial Neural Network)
- ANNs are computational models inspired by the **biological structure** and **functions** of the human brain.
- ANNs are composed of interconnected nodes **(neurons)** that process information **(signals)**.
- Each neuron receives signals, processes those signals, and then sends its signals to other neurons.
- Designed to recognize patterns and solve complex problems by learning from data.
- **Neurons:** The fundamental unit, receives inputs, processes them, and produces an output.

### Layers 
Neurons are organized into interconnected layers.
1. **Input Layer:** Receives data as an input (a vector of numerical values).
2. **Hidden Layer:** Process and transform the data. Sends it to the subsequent nodes/layers.
3. **Output Layer:** Produces the final result.
- **Weights:** Each connection between neurons has a weight (strength of the connection)
- **Biases:** Added to the weighted sum of inputs to adjust the neuron's output.
- **Activation Function:** A mathematical function that determines the output of a neuron based on its input.
- **Learning process:** ANN learns by adjusting their weights and biases through backpropagation.
- **Backpropagation:** Compares the network's output to the desired output and updates the weights to minimize the error. 

### Example: Image Recognition
Imagine training an ANN to recognize handwritten digits.

1. **Input:** 
- The image of a handwritten digit is divided into a grid of pixels, and the pixel values are fed to the input layer.

2. **Hidden layers:** 
- The hidden layers process the input data, extracting features like edges, curves, and shapes.

3. **Output layer:** 
- The output layer produces a probability distribution for each digit (0-9).
- The digit with the highest probability is considered the network's prediction.

4. **Training:** 
- The network is trained on a dataset of handwritten digits.
- During training, the weights and biases are adjusted to minimize the error between the predicted output and the correct label.

### FNN (Feed Forward Network)
- The simplest type of ANN, information flows in one direction, from the input to the output layer without any feedback loops.
- **Single layer perceptron (SLP):** A simple network with only one hidden layer.
- **Multi-layer perceptron (MLP):** A network with multiple hidden layers, capable of learning complex patterns.

### DNN (Deep Neural Network)
- A type of ANN with multiple hidden layers between the input and output layers.
- The **"deep"** refers to the depth that allows DNNs to learn complex patterns and relationships in the data.
- A DNN can learn to identify the pattern by breaking the data (image) into smaller features.
- The deeper layers of the network can then combine these features to form a more complex understanding.
- **Input Layer:** The first layer receives the input data, such as an image or a text document.
- **Hidden Layers:** These layers process the input data, learn the useful features and extract them.
- Each neuron in a hidden layer is connected to neurons in the previous and subsequent layers.
- The weights on these connections determine how much influence each neuron has on the others.
- **Output Layer:** The final layer produces the output, such as a classification or a prediction.

### CNN (Convolutional Neural Network)
- A type of ANN specialized for processing and analyzing grid-like data such as images and video.
- They have convolutional layers that automatically and adaptively learn spatial hierarchies of features.
- **Use Cases:** Computer Vision tasks like object detection, image classification, and segmentation.
- **Basic Idea:** Use convolution operations to process data in small chunks (like small image patches)

### Key Components of CNNs
1. **Convolutional Layers:** 
- These layers apply filters to the input data, extracting basic features like edges, corners, and textures.
- The filters are essentially small matrices that slide across the input image, computing the dot product with the underlying pixels.
- Subsequent layers can extract more complex features, such as the shape of the animal's head, body, and tail.

2. **Pooling Layers:** 
- These layers downsample the feature maps, reducing the dimensionality of the data while preserving the most important information.

3. **Fully Connected Layers:** 
- The final layers combine the extracted features to produce a probability for each class (cat or dog).
- The class with the highest probability is chosen as the prediction.

### RNN (Recurrent Neural Network)
- A type of ANN designed to process sequential data like time series, video, audio and sentences (sequence of words/texts)
- A type of neural network where connections between nodes form a cycle, allowing output from previous steps to influence the current step.
- **Hidden State:** RNN maintains a hidden state, representing the network memory of previous/past input.
- **Recurrent Connections:** Allows information to flow from the previous node to the current node to capture dependencies and context.

### LSTM (Long Short-Term Memory)
- A special type of RNN design to address the vanishing gradient problem while dealing with long sequences.
- The vanishing gradient problem is a phenomenon that occurs during the training of deep neural networks.
- The gradients that are used to update the network become extremely small (vanish) as they are backpropagated.
- LSTM is a powerful tool for modelling sequential data and capturing long-term dependencies.
- LSTM introduces a memory cell to each hidden layer. Three gates control the memory cell.
- These memory cells help the network to remember information over a long period selectively.
- **Forget Gate:** Determines how much of the previous cell state should be forgotten (Things to forget)
- **Input Gate:** Determines how much of the current input should be written to the cell state (Things to remember)
- **Output Gate:** Determines how much of the cell state should be sent as output.
- **Application:** NLP, Speech Recognition, Time Series Analysis, Music Generation, etc.
