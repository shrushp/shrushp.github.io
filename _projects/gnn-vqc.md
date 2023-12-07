---
layout: page
title: Hybrid Quantum-Classical Graph Neural Networks
description: Hybrid GNN-VQC model for image classification
img: assets/img/GNN_VQC.png

importance: 1
category: Major
related_publications: ray2023hybrid
---

Understanding how tumor cells self-organize and interact within the tumor microenvironment (TME) is a long standing question in cancer Biology. In This project, we modelled TME as a graph structure to comprehensively encode the tissue composition in terms of biologically meaningful entities, such as cells, tissues, and their interactions. As a result, GNNs can elegantly integrate cellular information with tumor morphology, topology, and interactions among cells and/or tissue structures. We created a hybrid classical-quantum network which combines a GNN with a Variational Quantum Classifier (VQC). 


<div class="row">
    <div class="col-sm mt-1 mt-md-0">
        {% include figure.html path="assets/img/GNN_VQC.png" title="Hybrid GNN" class="img-fluid rounded z-depth-1" style="width: 20px; height: auto;" %}
    </div>
</div>
<div class="caption">
   Implementation of hybrid GNN-VQC model.
</div>

We followed two approaches for training our Hybrid Network with different encoding schemes and feature dimensions: 

(i) with a pretrained GNN (having frozen weights)

(ii) with trainable GNN and VQC parameters to backpropogate simultaneously.

<div class="row">
    <div class="col-sm mt-1 mt-md-0">
        {% include figure.html path="assets/img/AEresults.png" title="results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Classical compression vs Quantum compression.
</div>

We showed that end-to-end training is significantly better than serially training such models and demonstrate results on a real-world breast-cancer subtyping task. In detailed ablation studies we observed that quantum compression can be significantly better to qubit requirements without information loss unlike lossy classical compression. Future directions could be to explore how other such classical networks can be combined with quantum circuits to enhance their trainability and improve generalization.


Source code: 


[End to end trainable GNN-VQC](https://github.com/Next-di-mension/end-to-end-trainable-GNN.git)


