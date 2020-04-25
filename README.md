# CarDent-Detection_Assessment

Facebook Research released pre-built Detectron2 versions, which make local installation a lot easier. (Tested on Linux and Windows)

Alongside the release of PyTorch version 1.3 Facebook also released a ground-up rewrite of their object detection framework Detectron. The new framework is called Detectron2 and is now implemented in PyTorch instead of Caffe2.

Detectron2 allows us to easily us and build object detection models. This article will help you get started with Detectron2 by learning how to use a pre-trained model for inferences as well as how to train your own model.

What's New

    It is powered by the PyTorch deep learning framework.
    Includes more features such as panoptic segmentation, densepose, Cascade R-CNN, rotated bounding boxes, etc.
    Can be used as a library to support different projects on top of it. We'll open source more research projects in this way.
    It trains much faster.


Semantic segmentation

Semantic segmentation refers to the process of linking each pixel in an image to a class label. These labels could include a person, car, flower, piece of furniture, etc., just to mention a few. We can think of semantic segmentation as image classification at a pixel level.

If you want to use a custom dataset while also reusing detectron2’s data loaders, you will need to

Register your dataset (i.e., tell detectron2 how to obtain your dataset). Optionally, register metadata for your dataset. Next, we explain the above two concepts in details.

The Colab Notebook has a working example of how to register and train on a dataset of custom formats.

