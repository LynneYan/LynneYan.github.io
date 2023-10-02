---
layout: page
title: project 2
description: Enhancing data reduction with topology 
img: assets/img/project2.png
importance: 2
category: 
related_publications: YanLiangGuo2023, yan2018homology
---

The disparity between the rapidly increasing computing performance and the slow increase in storage and I/O bandwidth of supercomputers necessitates data compression, where data produced by simulations are compressed in situ and decompressed in situ and post hoc for analysis and exploration. However, most of today’s lossy compressors (e.g., ZFP, FPZIP, SZ, etc.) provide global error bounds on the decompressed data, which do not guarantee the preservation of topological features essential to scientific discoveries. We worked on developing advanced data reduction techniques and software that preserve topological features in data for in situ and post hoc analysis and visualization at extreme scales. 

<div class="row justify-content-sm-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project2-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project2-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Eliminate topological false cases with iterations. Right: 3D visualization of original and decompressed data with different parameter settings. Images from <a href='https://arxiv.org/abs/2304.11768' style="color: blue">[VIS23b]</a>.
</div>

We designed and led the development of TopoSZ <a href='https://arxiv.org/abs/2304.11768' style="color: blue">[VIS23b]</a>, an error-bounded lossy compression method that preserves the topological features in 2D and 3D scalar fields. The main idea is to derive topological constraints from contour-tree-induced segmentation from the data domain and incorporate such constraints with a customized error-controlled quantization strategy from the SZ compressor. Our method allows users to control the pointwise error and the loss of topological features during compression. 


<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project2-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project2-4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Homology-preserving dimensionality reduction using manifold landmarking: original point clouds, Isomap embeddings, random landmark Isomap embeddings, and homological landmark Isomap embeddings. Right: original point cloud, Isomap embeddings without tearing, with partial tearing and with the optimal tearing, respectively. Images from <a href='https://arxiv.org/abs/1806.08460' style="color: blue">[VDS18]</a>.
</div>

Another example is HIsomap <a href='https://arxiv.org/abs/1806.08460' style="color: blue">[VDS18]</a>, a topology-preserving dimensionality reduction (DR) technique for high-dimensional point clouds. It uses the data skeleton based on the mapper graph, a type of topological descriptor, to select landmarks and integrate these landmarks with the classic DR technique Isomap to preserve topology. 