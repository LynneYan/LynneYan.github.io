---
layout: page
title: project 3
description: Mitigating uncertainty with topology
img: assets/img/project3.png
importance: 3
category:
related_publications: yan2019structural, athawale2020uncertainty, yan2021scalar, YanMasoodRasheed2023

---
I envision new methodologies to quantify, visualize, and mitigate data uncertainties by combining topological, geometric, statistical, and visualization techniques. Uncertainty visualization is a very active area of research. Uncertainty information is often summarized via statistical quantities (such as mean, median, and standard deviation) and encoded with data via color, opacity, texture, glyphs, animation, etc. The challenges associated with the study of structure-wise uncertainty in graph-based descriptors can be attributed, in part, to the difficulty in characterizing and quantifying their structural uncertainty. In particular, ensemble datasets combining multiple realizations of a phenomenon are often used to mitigate the effects of uncertainty. 

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project3-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project3-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: User interface for the interactive visualization of labeled merge trees and their 1-center. Right: 2D projections of vertex consistency visualization of an ensemble of neuron trees reconstructed from OP 6. Images from <a href='https://ieeexplore.ieee.org/document/8794553' style="color: blue">[VIS19]</a>.
</div>

We designed and led the development of an interactive visualization system resembling a numerical calculator that takes a set of merge trees as input and outputs a tree as their structural average <a href='https://ieeexplore.ieee.org/document/8794553' style="color: blue">[VIS19]</a>. This visualization tool can highlight structural similarities between the input and the average and incorporate uncertainty information for visual exploration. Our proposed uncertainty visualization measure can be used to understand structural variations among merge trees arising from scalar field ensembles. For example, I used these proposed methodologies to help study differences/variations among different reconstructions of the same neuron cell. 


<div class="row justify-content-sm-center">
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project3-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project3-4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project3-5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.html path="assets/img/project3-6.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left to Right: Ensemble members at time steps 60, 63, and 66, and Morse complex of the mean field. Images from <a href='https://ieeexplore.ieee.org/document/9187994' style="color: blue">[TVCG20]</a>..
</div>

Another example is statistical summary maps for quantifying structural variations and visualizing positional uncertainties of Morse complexes in ensembles <a href='https://ieeexplore.ieee.org/document/9187994' style="color: blue">[TVCG20]</a>. Specifically, we introduced three types of statistical summary maps – the probabilistic, significance, and survival maps – to characterize the uncertain behaviors of gradient flows. We demonstrated the utility of our proposed approach using wind, flow, and ocean eddy simulation datasets. 
