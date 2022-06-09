---
layout: page
title: Are Neural Networks Excessively Invariant?
description: Course project
img: assets/img/branch_pic.png
html: assets/pdf/nn_invar_project_report.pdf
importance: 2
category: work
---

<a href="assets/pdf/nn_invar_project_report.pdf" class="btn btn-sm z-depth-1" role="button">Link to report</a>  <a href="https://github.com/SriramB-98/null-invar" class="btn btn-sm z-depth-1" role="button">Link to code</a>

Despite the remarkable success of deep neural networks in a myriad of settings, several works have demonstrated their vulnerability to imperceptible perturbations, known as adversarial attacks. On the other hand, prior works have also demonstrated the excessive insensitivity of deep networks to large-magnitude perturbations in input space. In light of these observations, we aim
to identify techniques to study the extent of excessive invariance displayed by deep neural networks.
Towards this, we propose a novel Null Space Projected Gradient Descent (NSPGD) attack, that
iteratively refines image perturbations without affecting network activations. Further, we study the
efficacy of confidence calibration of classification networks as a mode to mitigate excessive invariance, in order to train models that are robust to such attacks, while simultaneously being robust to standard adversarial attacks.




<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/island_pic" title="Island scenario" class="img-fluid rounded z-depth-1" %}
    </div>
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/branch_pic.png" title="Branch scenario" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Left: </b> Decision boundaries of a model that is excessively sensitive but not excessively invariant (“island-like”) <br /> 
    <b>Right: </b> Decision boundaries of a model that is excessively sensitive and excessively invariant (“branch-like”)
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/cifar10_at_path.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/cifar10_normal_path.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    Visualization of the equi-confidence paths. The 95th (purple-orange) and 5th (blue-green) percentile confidences are plotted for each image and each radius.
</div>

Although adversarial training reduces the number of adversarial examples within the $$\epsilon$$ ball, the equi-confidence paths are much wider for adversarial models. This could be because adversarial models are smoother as compared to normally trained models, thus they are more invariant in directions normal to the tangent vector at that point.

For more details, please refer to the project report and code.