# Image Recognition with VGG16 and MobileNet

This repository showcases two image classification pipelines using the Keras API integrated in TensorFlow (tf.keras):

- **VGG16** for classifying cats vs. dogs
- **MobileNet** for recognizing hand sign digits (0–9)

Both implementations demonstrate transfer learning, custom image preprocessing and evaluation


## Project Files

| File | Task | Description |
|------|------|-------------|
| `ImageCNN.ipynb` | Cats vs Dogs | Uses `tf.keras.applications.VGG16` for transfer learning on a custom cats vs. dogs dataset. Includes directory structuring and image data augmentation. |
| `MobileNet.ipynb` | Hand Sign Digit Recognition | Uses `tf.keras.applications.MobileNet` to classify hand gestures representing digits 0–9. Includes manual image preprocessing and inference logic. |

##  Key Concepts

-  TensorFlow Keras API for model definition, training, and evaluation
-  Transfer Learning with pretrained `VGG16` and `MobileNet`
-  Image Preprocessing 
-  Custom inference pipelines for single image prediction


## VGG16 – Cats vs Dogs

- Dataset: Balanced subset of 1,000 training, 200 validation, and 100 test images
- Architecture: VGG16 (without top), used for feature extraction
- Preprocessing: Directory-based image loading with `ImageDataGenerator`

---

## MobileNet – Sign Language Digits

- Dataset: Static hand sign digit images stored in a local folder
- Architecture: Lightweight MobileNet for efficient inference
- Preprocessing: Manual resizing and normalization to fit input size `(224, 224)`
