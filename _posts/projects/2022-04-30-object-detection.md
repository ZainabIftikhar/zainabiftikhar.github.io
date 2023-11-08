---
layout: post
title: Attention-Based Object Detection
categories: projects
permalink: projects/attention-based-object-detection
authors: Zainab Iftikhar
---
    
<p> Producing a set of bounding boxes and category labels around objects detected in images using a CNN-encoder-decoder backbone.
<em> DL 2022 </em></p>

----

## Abstract

<p> Object detection algorithms are critically important for applications as diverse as self-driving cars, face recognition, motion tracking, and pedestrian monitoring, making it critical to develop object detection algorithms that are accurate yet architecturally simple
and scalable. This project reimplement the novel object detection algorithm presented in “End-to-End Object Detection with Transformers”The model produces a set of bounding boxes and category labels around objects detected in images using a CNN-encoder-decoder backbone. </p>

<p> The model uses the Microsoft Common Objects in Context (COCO) 2017 detection dataset (118K Training Images, 5K Validation Images). The ground truth labels for the object detection task were: Bounding box coordinates (x, y, w, h) and Class Labels for each bounding box. Each image has at least one bounding box annotation with an average of 7 bounding boxes per image and a maximum of 63.</p>

<p>The model relies on a framework called a <b> DEtection TRansformer (DETR) </b> and uses a bipartite matching function and Hungarian loss to train the model. However, we found that the model is not translate-able. The model was only suitable only for inference or training with distributed/parallel training. The DeTR framework is relatively recent with multiple aspects of novelty which made the pytorch-tensorflow translation quite challenging.</p>

----

## Poster

<embed src="/assets/projects/dl_object_detection.pdf" type="application/pdf" width="100%" height="500px" />


[Click here for a full-screen view.](/assets/projects/dl_object_detection.pdf)

---
