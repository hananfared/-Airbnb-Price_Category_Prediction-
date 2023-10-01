# -Airbnb-Price_Category_Prediction-

1.   ## **Is fully-connected model a good one for sequential data? Why? How about for image data? Is it good? Why?**

> **Ans:** A fully-connected neural network, also known as a dense neural network, is a good choice for sequential data processing when the sequence is relatively short and the relationship between elements in the sequence is simple, such as in sentiment analysis or text classification tasks. However, for longer and more complex sequential data, such as natural language processing, speech recognition, or language translation, other models such as recurrent neural networks (RNNs) or transformers are more commonly used, as they can capture the temporal dependencies and long-term dependencies in the sequence.

- For image data, fully-connected networks are not typically used as they require a fixed input size, which is not practical for images of varying sizes. Instead, convolutional neural networks (CNNs) are more commonly used for image classification, object detection, and other image-related tasks. CNNs are well-suited for image data because they are able to learn spatial features through their convolutional layers, and are able to handle inputs of varying sizes through the use of pooling and other techniques.
