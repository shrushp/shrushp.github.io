---
layout: page
title: Solving CO problems through VQA and unsupervised clustering
description: Masters thesis
img: assets/img/tn.png

importance: 3
category: Major
related_publications: patil2023measurementbased
---

> How would you determine the ground state of a quantum system with no exact solution?
> - Dr. Sheldon Cooper


For my thesis, I joined lab of Prof. Prasanta Panigrahi at IISER Kolkata and worked on solving large scale combinatorial optimization problems through clustering methods.

Together, we developed two novel clustering algorithms, one being a quantum algorithm following divisive approach and the other being inspired by unsharp measurements. Following blocks show the workflow of developed algorithms. 

## Heirarchical Quantum Clustering Algorithm

{% raw %}
```python
    Input: {D_{k_1i}}, n, m
    Output:  k  clusters
    initialization
    Construct the state  |ψ>
    for num_clusters !=  k 
    |    apply  U  on n + m register if num clusters = k then
    |    |   Return: Output
    |    else
    |    |    further split the clusters by applying U or merege until num clusters = k
    |    end
    end

```
{% endraw %}

## Unsharp measurement based Clustering Algorithm

{% raw %}
```python
    Input: {D_{k_1i}}, n
    Output: k clusters
    initialization
    Construct the superposed quantum state as described
    for cluster around point i do
    |    measure state unsharply around i if num clusters = k
    |    then
    |    |    Return: Output
    |    else
    |    |    re-center the next distance j at i and measure until num clusters = k
    |    end
    end
```
{% endraw %}

We implemented them on various datasest for the benchmarking purpose and found that it outperforms state-of-the-art quantum clustering algorithms as well as classical divisive clustering. Below are the results. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/conc_cir_input.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/conc_circile_output_classical.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/concentric_circle_output_algo_1.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
</div>
<div class="caption">
    (Left) Dataset of 400 points generated using sklearn with noise ratio of 0.1. (Middle) Classification of the dataset using the traditional classical divisive clustering algorithm. (Right) Classification of the dataset using the QHCA. Different colors represent different clusters. 
</div>
The main goal of thesis was to solve large scale graph problems like TSP; we employed two methods:

(i) one is implenting developed algorithms to  cluster the nearby cities in TSP data. 

<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/city_data.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/city_out.png" title="example image" class="img-fluid z-depth-1" %}
    </div>
</div>
<div class="caption">
    (Left) Original TSP dataset of 130 cities (Right) Radially clustered data
</div>

(ii) and the second using tensor networks. 






