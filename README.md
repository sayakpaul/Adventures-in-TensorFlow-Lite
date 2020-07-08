# Adventures-in-TensorFlow-Lite
This repository contains notebooks that show the usage of TensorFlow Lite for quantizing deep neural networks in TensorFlow 2. ***It is currently under active development so, there might be some inconsistencies in the description below***. 

![](https://www.tensorflow.org/site-assets/images/project-logos/tensorflow-lite-logo-social.png)

## About the notebooks
- `A_tale_of_quantization.ipynb`: A comprehensive notebook showing different ways to quantize a model in `tf.keras` (with fine-tuning). It includes both **quantization-aware training** as well as **post-training quantization**. This notebook is accompanied by [this report](https://bit.ly/3dlCRSI) that has some additional details and performance considerations. The notebook is best referred with this report. 
- `Custom_Image_Classification_EdgeTPU.ipynb`: It shows how to use post-training quantization with a representative dataset to calibrate the dynamic ranges of activations. It also shows how to quantize the model in a way that is compatible with an Edge TPU USB Accelerator. 
- The others to be updated

## References
- [Post-training quantization](https://www.tensorflow.org/lite/performance/post_training_quantization)
- [Quantization aware training with TensorFlow Model Optimization Toolkit](https://blog.tensorflow.org/2020/04/quantization-aware-training-with-tensorflow-model-optimization-toolkit.html)

## An accompanying deck on TensorFlow Lite
- I often talk about TensorFlow Lite and here's the deck I mostly use: http://bit.ly/tfl-pune. 

## Acknowledgements
- [Arun Venkatesan](https://www.linkedin.com/in/arun-venkatesan-9317796/)
- [Khanh LeViet](https://www.linkedin.com/in/lvgk/)
- [Pulkit Bhuwalka](https://www.linkedin.com/in/pulkitbhuwalka/)
