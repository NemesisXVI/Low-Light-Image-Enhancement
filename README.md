# Low Light Image Enhancement

With the goal of recovering high-quality image content from its degraded version, image restoration enjoys numerous applications, such as in photography, security, medical imaging, and remote sensing. In this example, we implement the MIRNet-v2 model for image enhancement, a fully-convolutional architecture that learns an enriched set of features that combines contextual information from multiple scales, while simultaneously preserving the high-resolution spatial details.

Although the MIRNet-v2 architecture can be applied to a variety of image restoration tasks such as single image denoising, super-resolution, image deblurring, etc, in this notebook we would demonstrate an implementation of this architecture for low-light image enhancement using TensorFlow.

- In this notebook we aim to demonstrate the task of Low-light Image Enhancement.
- The ideas used to implement the code was proposed by the paper [Learning Enriched Features for Fast Image Restoration and Enhancement](https://www.waqaszamir.com/publication/zamir-2022-mirnetv2/zamir-2022-mirnetv2.pdf).
- We implement the model and training pipeline using Tensorflow and Keras.
- We use Weights and Biases for tracking the losses and metrics of our experiment in real-time and storing model checkpoints as artifacts.
