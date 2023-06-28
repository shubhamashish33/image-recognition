
# **Image Recognition using Various Known Predefined Models**
For this purpose of study I have selected to model which are widely popular and known as well.
- TensorFlow Kera
- Pytorch (using YOLO)
Both of Them are good and well implemented model which can be used for faster processing and development.

## Keras
Keras is the high-level API of the TensorFlow platform. It provides an approachable, highly-productive interface for solving machine learning (ML) problems, with a focus on modern deep learning. Keras covers every step of the machine learning workflow, from data processing to hyperparameter tuning to deployment. It was developed with a focus on enabling fast experimentation.

With Keras, you have full access to the scalability and cross-platform capabilities of TensorFlow. You can run Keras on a TPU Pod or large clusters of GPUs, and you can export Keras models to run in the browser or on mobile devices. You can also serve Keras models via a web API.

Keras is designed to reduce cognitive load by achieving the following goals:

 - Offer simple, consistent interfaces.
 - Minimize the number of actions required for common use cases.
 - Provide clear, actionable error messages.
 - Follow the principle of progressive disclosure of complexity: It's easy to get started, and you can complete advanced workflows by learning as you go.
 - Help you write concise, readable code.

More you can Read it ![Here ](https://www.tensorflow.org/guide/keras)

## YOLO
YOLOS is a Vision Transformer (ViT) trained using the DETR loss. Despite its simplicity, a base-sized YOLOS model is able to achieve 42 AP on COCO validation 2017 (similar to DETR and more complex frameworks such as Faster R-CNN).

The model is trained using a "bipartite matching loss": one compares the predicted classes + bounding boxes of each of the N = 100 object queries to the ground truth annotations, padded up to the same length N (so if an image only contains 4 objects, 96 annotations will just have a "no object" as class and "no bounding box" as bounding box). The Hungarian matching algorithm is used to create an optimal one-to-one mapping between each of the N queries and each of the N annotations. Next, standard cross-entropy (for the classes) and a linear combination of the L1 and generalized IoU loss (for the bounding boxes) are used to optimize the parameters of the model.

More you can Read it ![Here](https://huggingface.co/hustvl/yolos-tiny)

Below are Implenetation code for both of the algorithms.

## Result
- Input Image used for this
![image](https://github.com/shubhamashish33/image-recognition/assets/78084828/10435bd0-c7e4-4fad-8fd1-ad053daaa5a8)


- TensorFlow \
![Screenshot from 2023-06-28 18-01-05](https://github.com/shubhamashish33/image-recognition/assets/78084828/be38dfa7-8f83-4471-8417-369ac5ea0c5d)

- YOLO
![Screenshot from 2023-06-28 18-03-52](https://github.com/shubhamashish33/image-recognition/assets/78084828/8319b66f-d8ef-4634-88ce-209051293b77)

## Conclusion

But **TensorFlow Kera** has found out to be better model than the YOLO.
