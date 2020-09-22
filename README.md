# Adventures-in-TensorFlow-Lite
This repository contains notebooks that show the usage of TensorFlow Lite (TF Lite) for quantizing deep neural networks in TensorFlow 2. ***It is currently under active development so, there might be some inconsistencies in the description below***. 

<br><div align="center">
  <img src="https://i.ibb.co/mbT8CZX/tensorflow-lite-logo-social-1.png"></img> <img src="https://i.ibb.co/ZXtwJjV/Webp-net-resizeimage.png"></img>
</div><br>

## About the notebooks
- `A_tale_of_quantization.ipynb`: A comprehensive notebook showing different ways to quantize a model in `tf.keras` (with fine-tuning). It includes both **quantization-aware training** as well as **post-training quantization**. This notebook is accompanied by [this report](https://bit.ly/3dlCRSI) that has some additional details and performance considerations. The notebook is best referred with this report. 
- `Custom_Image_Classification_EdgeTPU.ipynb`: It shows how to use post-training quantization with a representative dataset to calibrate the dynamic ranges of activations. It also shows how to quantize the model in a way that is compatible with an Edge TPU USB Accelerator. 
- `DeepLabV3/DeepLab_TFLite_*.ipynb`: These notebooks show how to convert several DeepLabV3 based segmentation models (trained on the PASCAL VOC 2012, ADE20k, and CityScapes datasets) to TF Lite and run inference with them.
- `ESRGAN_TFLite.ipynb`: Shows how to run inference with this ESRGAN module from TF Hub, convert it to TF Lite, run inference with the model. A bonus includes running inference with a distilled version of the main model (only 33 KB).
- `Magenta_arbitrary_style_transfer_model_conversion.ipynb`: Shows to how apply apply different post-training quantization schemes to the [arbitrary style transfer model provided by Magenta](https://github.com/magenta/magenta/tree/f3b66aa1354cd933f0e9757a567cc9a3d2d03297/magenta/models/arbitrary_image_stylization). This generates image stylization models that produce higher-quality images than [these ones](https://tfhub.dev/google/magenta/arbitrary-image-stylization-v1-256/2). Inference notebook is available here - `Style_Transfer_Demo_InceptionV3.ipynb`. Additionally, in this notebook you can find how to run inference with the same TF Lite models but with dynamic shape support: `Style_Transfer_Demo_InceptionV3_Dynamic_Shape.ipynb`. 
- `Model_Pruning_in_Deep_Learning_with_tfmot.ipynb`: Shows how to use the pruning APIs of TensorFlow Model Optimization toolkit along with TF Lite.
- `Selfie2Anime_TFLite(50_Checkpoints).ipynb`: Shows how to convert the [UGATIT model](https://github.com/taki0112/UGATIT) (also known as Selfie2Anime GAN) to TF Lite. Inference notebook is available [here](https://github.com/margaretmz/selfie2anime-e2e-tutorial/blob/master/ml/Selfie2Anime_Model_Conversion_50_Epochs.ipynb). Here's a multi-part tutorial of this project - [Part I](https://bit.ly/selfie2anime-1), [Part II](https://bit.ly/selfie2anime-2), [Part III](https://bit.ly/selfie2anime-3). This was jointly done with [Margaret](https://twitter.com/margaretmz). 
- `Semantic_Segmentation_+_Background_Removal_+_Style_Transfer.ipynb`: Presents a demo on how to use multiple TF Lite models to run segmentation, remove background, and apply stylization. 
- `Style_Transfer_Demo.ipynb` & `Style_Transfer_Demo_InceptionV3.ipynb`: Present interactive image stylization demos. 
- `TUNIT_Conversion_to_TF_Lite.ipynb`: Shows the PyTorch -> TF Lite model conversion worflow (this is currently buggy).
- `CartoonGAN_TFLite.ipynb`: Shows to how to convert the CartoonGAN model (proposed [here](https://bit.ly/cartoon-gan)) to a TF Lite model. Includes how to run inference as well. Here's the [official TensorFlow blog](https://github.com/SystemErrorWang/White-box-Cartoonization) in case you are interested to know more. 

## References
- [Post-training quantization](https://www.tensorflow.org/lite/performance/post_training_quantization)
- [Quantization aware training with TensorFlow Model Optimization Toolkit](https://blog.tensorflow.org/2020/04/quantization-aware-training-with-tensorflow-model-optimization-toolkit.html)

## Accompanying materials
- [Doing more with TF Lite](http://bit.ly/tfl-pune)
- [Model optimization 101](http://bit.ly/mo-101)
- [A few good stuff in TF Lite](http://bit.ly/stuff-tflite)
- [A Tale of Model Quantization in TF Lite](https://bit.ly/3dlCRSI)
- [Plunging into Model Pruning in Deep Learning](https://bit.ly/2AJ67W4)

## Find the models on TF Hub

https://tfhub.dev/s?publisher=sayakpaul

![](https://i.ibb.co/zJSFjPs/Screen-Shot-2020-07-11-at-3-14-52-PM.png)


## Acknowledgements
- [Arun Venkatesan](https://www.linkedin.com/in/arun-venkatesan-9317796/)
- [Khanh LeViet](https://www.linkedin.com/in/lvgk/)
- [Pulkit Bhuwalka](https://www.linkedin.com/in/pulkitbhuwalka/)
