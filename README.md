# AI Ear
TITLE : AiEar
PROBLEM STATEMENT: Classifying different types of audio using DeepLearning models
EXPLANATION:
Iam using librosa ,resampy , relu , softmax and tensorflow keras model for the successful implementation of my project.

Workflow: 
librosa library : open source library helps in music and sound extraction and analysis. it also helps in maintaining records. it helps in extracton of features like burden sound from a circle, register of different spectrogram portrayals, symphonious percussive source detachment, etc.


Two types of sound:
Mono sound signals and stereo


Librosa converts into mono with 22khz sample rate and stereo into mono.
wavfile from scipy keeps it in original sample rate and stereo only


audio data is the numeric values of the waveform of a sound wave


Now we extract features through Mel-Frequency Cepstral Coefficients(MFCC) . Features extracted from patterns in frequency and time characteristics.


FEATURE EXTRACTOR:
librosa.load takes out audio data and sample rate
scaled features are extracted by taking mean of the transpose of mfccs 


We're gonna use tensorflow .
sequential model from tensorflow.


3 +1 layers. Activation function - relu
final layer is Dense layer.it will have softmax because its multilayer classification
Dropout is used to prevent over fitting. Regularisation technique r


then train tensorflow model. use test dataset and so some prediction
we run the model for 200 epochs

Librosa : Librosa is a Python package for music and audio analysis. It provides tools for tasks such as loading audio files, extracting features from audio signals, and performing various analyses like spectral decomposition and beat tracking. Librosa is widely used in music information retrieval, audio signal processing, and machine learning applications related to sound and music. Its user-friendly interface and extensive documentation make it a popular choice among researchers, students, and developers working on projects involving audio data. Librosa facilitates tasks such as audio classification, genre recognition, music recommendation, and more, making it a valuable tool in the field of digital signal processing and music analysis.

resampy : 
Resampy is a Python library primarily used for high-quality audio resampling. Resampling is the process of changing the sampling rate of a digital signal, such as audio, while preserving its essential characteristics. Resampy offers efficient resampling algorithms that maintain signal fidelity and minimize distortion during the conversion process.

This library is particularly useful in audio processing tasks where signals with different sampling rates need to be aligned or processed together. It provides a range of resampling methods, including interpolation-based techniques like linear interpolation and sinc-based resampling, which are well-suited for audio applications.

Resampy is often used in conjunction with other audio processing libraries, such as Librosa, to handle tasks like loading audio files with different sampling rates and converting them to a consistent format for further analysis or processing. Its straightforward interface and robust performance make it a valuable tool for developers and researchers working on audio-related projects.

relU:
ReLU, or Rectified Linear Unit, is a popular activation function used in artificial neural networks, particularly in deep learning models. It is a simple yet effective non-linear function that introduces non-linearity to the neural network, enabling it to learn complex patterns and relationships in data.

The ReLU function is defined as:

f(x)=max(0,x)

In other words, ReLU returns the input 
x if it is greater than zero, and zero otherwise. This means that ReLU effectively acts as a thresholding function, outputting zero for negative inputs and leaving positive inputs unchanged.

Softmax:
Softmax is a mathematical function often used in machine learning, particularly in classification tasks where the goal is to assign probabilities to multiple classes. It takes as input a vector of real numbers and outputs a probability distribution over multiple classes, ensuring that the probabilities sum up to 1.

Keras :
Keras is an open-source neural network library written in Python. It is known for its user-friendliness, modularity, and ease of use, making it a popular choice among beginners and experts alike for building deep learning models. TensorFlow, on the other hand, is an open-source machine learning framework developed by Google. Initially released in 2015, TensorFlow provides a flexible ecosystem of tools and resources for machine learning and deep learning tasks.

Keras and TensorFlow are closely related, with Keras originally being an independent project before being integrated into TensorFlow as its high-level API. This integration has led to the development of TensorFlow 2.0 and above, where Keras serves as the default high-level interface for building and training deep learning models within TensorFlow.

Key features and benefits of using Keras with TensorFlow include:

Simplicity and ease of use: Keras provides a simple and intuitive interface for building neural networks, allowing users to quickly prototype and experiment with different architectures.

Modularity and flexibility: Keras offers a modular design, making it easy to assemble complex neural networks from pre-built building blocks called layers. Users can customize and extend models with ease.

Compatibility: Keras is tightly integrated with TensorFlow, leveraging its computational backend for efficient execution on CPUs and GPUs. This integration ensures compatibility with other TensorFlow features and tools.

Extensibility: While Keras provides a high-level interface for building neural networks, TensorFlow's lower-level capabilities can still be accessed and utilized within Keras models, enabling users to implement custom operations and functionalities when needed.

Community and support: Both Keras and TensorFlow have large and active communities, offering extensive documentation, tutorials, and resources for learning and troubleshooting.

Overall, Keras with TensorFlow provides a powerful and versatile platform for developing deep learning models, suitable for a wide range of applications, from image and text processing to reinforcement learning and beyond.

Dataset link :  https://urbansounddataset.weebly.com/download-urbansound8k.html

