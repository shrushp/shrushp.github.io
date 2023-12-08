---
layout: page
title: Haar-Wavelet inspired Quanvolutional filter
description: Quantum Haar-Wavelet convolution 
img: assets/img/qhw.png
importance: 4
category: Minor
---

We propose a hybrid model; consisting of two sections: a quanvolutional filter part and then a classical layer part. First, we create a quanvolutional filter. a transformational layer called a ``quanvolutional layer,” which operates on input data by locally transforming the data using random quantum circuits, similar to the transformations performed by random convolutional filter layers. Quanvolutional layers apply random quantum circuits to input data, enabling local transformations and feature extraction.

The nice thing about Haar is that it doesn’t introduce any new artificial features; unlike others. That is the reason it is used by FBI to extract fingerprint analysis to extract characteristic information for each individual.
In the standard practice, we compute the power at each level to determine the dominant variations and extract physical information from the same.


<div class="row">
    <div class="col-sm mt-1 mt-md-0">
        {% include figure.html path="assets/img/QNN.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
</div>
<div class="caption">
    Developed hybrid model with Haar-filter.
</div>

<div class="row">
    <div class="col-sm mt-1 mt-md-0">
        {% include figure.html path="assets/img/QHW_circ.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
</div>
<div class="caption">
    Circuit representation of quantum Haar wavelet transforms. 
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm mt-1 mt-md-0">
        {% include figure.html path="assets/img/convolutions_generated.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
</div>
<div class="caption">
    Convolutions generated from each channel
</div>

Source code: 

[Haar wavlet inspired quantum convolutional filter](https://github.com/Next-di-mension/end-to-end-trainable-GNN.git)
