---
layout: default
modal-id: 5
date: 2020-06-16
img: uncertainty.gif
alt: image-alt
project-date: June 2020
conference: IEEE Conference on Computer Vision and Pattern Recognition
short: CVPR2020
keywords: [Confidence Estimation -, Monocular Depth Estimation -, Deep Learning] 
title: On the uncertainty of self-supervised monocular depth estimation
authors: [M. Poggi, F. Aleotti, F. Tosi and S. Mattoccia]
---

Self-supervised paradigms for monocular depth estimation are very appealing since they do not require ground truth annotations at all. 
Despite the astonishing results yielded by such methodologies, learning to reason about the uncertainty of the estimated depth maps is of paramount importance for practical applications, yet uncharted in the literature. 
Purposely, we explore for the first time how to estimate the uncertainty for this task and how this affects depth accuracy, proposing a novel peculiar technique specifically designed for self-supervised approaches. 
On the standard KITTI dataset, we exhaustively assess the performance of each method with different self-supervised paradigms. Such evaluation highlights that our proposal i) always improves depth accuracy significantly and ii) yields state-of-the-art results concerning uncertainty estimation when training on sequences and competitive results uniquely deploying stereo pairs.


<iframe width="640" height="360" src="https://www.youtube.com/embed/bxVPXqf4zt4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<div class="mx-auto" style="margin-bottom:-100px; margin-top:7%">
    <ul class="list-inline">
        <li>
            <a  style="color:#{{site.color.primary}};" href="https://github.com/mattpoggi/mono-uncertainty" class="btn-social btn-outline"><i class="fa fa-2x fa-github"></i></a>
        </li>
        <li>
            <a  style="color:#{{site.color.primary}}; " href="https://arxiv.org/pdf/2005.06209.pdf" class="btn-social btn-outline"><i class="fa fa-print fa-2x"></i></a>
        </li>
        <li>
            <a  style="color:#{{site.color.primary}};" data-dismiss="modal" class="btn-social btn-outline"><i class="fa fa-times fa-2x"></i></a>
        </li>
    </ul>
</div>

If you find the code useful, please cite our paper:
<div id="reference">
@inproceedings{Poggi_CVPR_2020,
title={On the uncertainty of self-supervised monocular depth estimation},
author={Poggi, Matteo and Aleotti, Filippo and Tosi, Fabio and Mattoccia, Stefano},
booktitle={IEEE Conference on Computer Vision and Pattern Recognition},
note={CVPR},
year={2020}
}
</div>
