# Concolutional Neural Network (CNN) Components In A Nutshell
1. **Generic Architecture**
  - Convolutional neural networks, also known as CNNs, are a specific type of neural networks 
  - that are generally composed of the following layers:
  - Input Image --> Convolutions(Filtering) --> Pooling (Feature Map)--> Fully Connected
2. **Layers**: Convolutional neural networks, also known as CNNs, are a specific type of neural networks that are generally composed of the following layers.
  - **Convolution Layer (CONV)**:The convolution layer (CONV) uses filters that perform convolution operations as it is scanning the input II with respect to its dimensions. 
    - Its hyperparameters include the filter size FF and stride SS. The resulting output OO is called feature map or activation map.
  - **Pooling (POOL)**: The pooling layer (POOL) is a downsampling operation, typically applied after a convolution layer, which does some spatial invariance. In particular, max and average pooling are special kinds of pooling where the maximum and average value is taken, respectively.
    - **Max Pooling**: Each pooling operation selects the maximum value of the current view.
      - Preserves detected features. It is most commonly used
    - **Average Pooling**: Each pooling operation averages the values of the current view
      - Downsamples feature map. It is used in LeNet
    - **Fully Connected (FC)**:The fully connected layer (FC) operates on a flattened input where each input is connected to all neurons. If present, FC layers are usually found towards the end of CNN architectures and can be used to optimize objectives such as class scores.
3. **Activation Functions**: decides whether a neuron should be activated or not. This means that it will decide whether the neuron's input to the network is important or not in the process of prediction using simpler mathematical operations.
  - Linear: $f(x) = x$
  - Tanh: $tanh(x)$
  - Rectified Linear Unit: $max(0, x)$
  - Sigmoid: $\sigma(x) = \frac{1}{1+e^{-x}}$
  - SOftmax: $p = \begin{bmatrix} p_1\\ .\\ .\\.\\p_n \end{bmatrix},\ where\ p_i = \frac{e^{x_i}}{sum_{j=1}^n e^{x_j}}$
5. **Hyperparameters Filtering**: The convolution layer contains filters for which it is important to know the meaning behind its hyperparameters.
  - **Dimensions of a filter**: A filter of size $F\times F$ applied to an input containing $C$ channels is a $F \times F \times C$ volume that performs convolutions on an input of size $I \times I \times C$ and produces an output feature map (also called activation map) of size $O \times O \times 1$.
    - Remark: the application of KK filters of size $F\times F$ results in an output feature map of size $O \times O \times K$.
  - 
6. **Hyperparameter Tuning**
7. **Fully Connected (FC)**:The fully connected layer (FC) operates on a flattened input where each input is connected to all neurons. If present, FC layers are usually found towards the end of CNN architectures and can be used to optimize objectives such as class scores.
  - 
8. **Applications**
  - 
