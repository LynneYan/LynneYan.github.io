---
layout: page
title: project 1
description: Redefining topology for domain-specific features
img: assets/img/project1.png
importance: 1
category: 
related_publications: YanUllrichVan-Roekel2022, YanGuoPeterka2023, YanMasoodRasheed2023, bujack2020state, yan2021scalar,
---


My vision is to tackle feature understanding by combining topological data analysis (TDA) and data visualization to support critical ingredients of a scientific workflow, including feature extraction, feature tracking, transitions, clusters, and periodicities detection. With the increasing gap between the complexity of large-scale scientific simulations and the limited bandwidth of human perceptions, TDA provides tools for scientific visualization in terms of abstraction and summarization. 


<div class="row justify-content-sm-center">
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project1-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project1-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project1-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left to right: feature tracking, selection, and comparison with the multilevel robustness framework. Images from <a href='https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.14799' style="color: blue">[CGF23]</a>.
</div>
We designed and led the development of TROPHY <a href='https://arxiv.org/abs/2307.15243' style="color: blue">[VIS23a]</a>, a framework that can improve the visual interpretability of vector fields in terms of feature tracking, selection, and comparison for large-scale scientific simulations. TROPHY was initially motivated by the lack of feature-tracking tools that consider closeness in structural stability instead of just distance proximity within the domain <a href='https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.14799' style="color: blue">[CGF23]</a>. It was then integrated with physical knowledge of tropical cyclones to drastically improve the computational efficiency of large-scale climate datasets <a href='https://arxiv.org/abs/2307.15243' style="color: blue">[VIS23a]</a>. TROPHY produced results comparable to (and sometimes even better than) those obtained with a widely used tropical cyclone tracking algorithm, requiring far fewer input data. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project1-4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Annually detected TCs by IBTrACS (1st column), TempestExtremes(2nd column), the TROPHY (3rd column) in 2004 (1st row) and 2009 (2nd row). Image from <a href='https://arxiv.org/abs/2307.15243' style="color: blue">[VIS23a]</a>.
</div>

Another example is a general and unifying two-step framework that supports geometry-aware comparisons of merge trees, a type of topological descriptors, for time-varying data <a href='https://ieeexplore.ieee.org/document/9744472' style="color: blue">[TVCG22]</a>. This framework can help detect transitions, clusters, and periodicities of a time-varying dataset and diagnose and highlight the topological changes between adjacent data instances. This framework also has the potential to study structural similarities and dissimilarities between scalar fields that arise from scientific simulations, with driving applications in cosmology, climate, and fusion simulations <a href='https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.14331' style="color: blue">[EuroVis21]</a>. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project1-5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Geometry-aware merge tree comparisons for transition detection. Image from <a href='https://ieeexplore.ieee.org/document/9744472' style="color: blue">[TVCG22]</a>.
</div>
