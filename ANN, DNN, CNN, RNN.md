# ANN | DNN | CNN | RNN

### ANN (Artificial Neural Network)
- ANNs are computational models inspired by the **biological structure** and **functions** of the human brain.
- ANNs are composed of interconnected nodes **(neurons)** that process information **(signals)**.
- Each neuron receives signals, processes those signals, and then sends its signals to other neurons.
- Designed to recognize patterns and solve complex problems by learning from data.
- **Neurons:** The fundamental unit, receives inputs, processes them, and produces an output.

### Layers 
Neurons are organized into interconnected layers.
1. **Input Layer:** Receives data as an input.
2. **Hidden Layer:** Process and transform the data. Sends it to the subsequent nodes/layers.
3. **Output Layer:** Produces the final result.
- **Weights:** Each connection between neurons has a weight (strength of the connection)
- **Biases:** Added to the weighted sum of inputs to adjust the neuron's output.
- **Activation Function:** A mathematical function that determines the output of a neuron based on its input.
- **Learning process:** ANN learns by adjusting their weights and biases through backpropagation.
- **Backpropagation:** Compares the network's output to the desired output and updates the weights to minimize the error. 

### **Example: Image Recognition**
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

### **FNN (Feed Forward Network)**
- The simplest type of ANN, information flows in one direction, from the input to the output layer without any feedback loops.
- **Single layer perceptron (SLP):** A simple network with only one hidden layer.
- **Multi-layer perceptron (MLP):** A network with multiple hidden layers, capable of learning complex patterns.
- **Radial basis function (RBF):** Uses RBF as an activation function, often used for interpolation and pattern recognition.

### **DNN (Deep Neural Network)**
- A type of ANN with multiple hidden layers between the input and output layers.
- The **"deep"** refers to the depth that allows DNNs to learn complex patterns and relationships in the data.
- A DNN can learn to identify the pattern by breaking the data (image) into smaller features.
- The deeper layers of the network can then combine these features to form a more complex understanding.
- **Input Layer:** The first layer receives the input data, such as an image or a text document.
- **Hidden Layers:** These layers process the input data, learn the useful features and extract them.
- Each neuron in a hidden layer is connected to neurons in the previous and subsequent layers.
- The weights on these connections determine how much influence each neuron has on the others.
- **Output Layer:** The final layer produces the output, such as a classification or a prediction.

### **CNN (Convolutional Neural Network)**
- A type of DNN specialized for processing grid-like data such as images and video.
- They have convolutional layers that automatically and adaptively learn spatial hierarchies of features.
- **Use Cases:** Image and video recognition, recommendation systems.
- **Basic Idea:** Use convolution operations to process data in small chunks (like small image patches)

### **RNN (Recurrent Neural Network)**
- RNNs are designed for sequential data like time series and sentences (sequence of words/texts)
- A type of neural network where connections between nodes form a cycle, allowing output from previous steps to influence the current step.
- **Use Cases:** Sequence prediction, time series forecasting, natural language processing.
- **Basic Idea:** Has memory from previous steps to inform the current step.

### **LSTM (Long Short-Term Memory)**
- A special type of RNN design to address the vanishing gradient problem while dealing with long sequences.
- LSTMs are a powerful tool for modelling sequential data and capturing long-term dependencies.
- LSTM introduces a memory cell to each hidden layer. The memory cell is controlled by three gates.
- These memory cells help the network to selectively remember information over long period of time.
- **Forget Gate:** Determines how much of the previous cell state should be forgotten.
- **Input Gate:** Determines how much of the current input should be written to the cell state (Things to remember)
- **Output Gate:** Determines how much of the cell state should be sent as output.
- **Application:** NLP, Speech Recognition, Time Series Analysis, Music Generation, etc.

### **LLM (Large Language Model)**
- A type of model that predicts the likelihood of a sequence of words.
- With the advancement in neural networks, modern LLMs like GPT (from OpenAI) and BERT (from Google) are neural-based and extremely powerful.
- **Use Cases:** Text generation, natural language understanding, question answering, and more.
- **Basic Idea:** Given a sequence of words, predict the next word or understand the context.
- It’s trained on large text corpora to understand and generate human-like text.
