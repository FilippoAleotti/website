---
layout: default
modal-id: 3
date: 2019-06-16
img: monoresmatch.gif
alt: image-alt
project-date: June 2019
conference: IEEE Conference on Computer Vision and Pattern Recognition
short: CVPR2019
keywords: [Monocular Depth Estimation -, Deep Learning] 
title: Learning monocular depth estimation infusing traditional stereo knowledge
authors: [Fabio Tosi, Filippo Aleotti, Matteo Poggi, Stefano Mattoccia]
---

Depth estimation from a single image represents a fascinating, yet challenging problem with countless applications. Recent works proved that this task could be learned without direct supervision from ground truth labels leveraging image synthesis on sequences or stereo pairs. Focusing on this second case, in this paper we leverage stereo matching in order to improve monocular depth estimation. To this aim we propose monoResMatch, a novel deep architecture designed to infer depth from a single input image by synthesizing features from a different point of view, horizontally aligned with the input image, performing stereo matching between the two cues. In contrast to previous works sharing this rationale, our network is the first trained end-to-end from scratch. Moreover, we show how obtaining proxy ground truth annotation through traditional stereo algorithms, such as Semi-Global Matching, enables more accurate monocular depth estimation still countering the need for expensive depth labels by keeping a self-supervised approach. Exhaustive experimental results prove how the synergy between i) the proposed monoResMatch architecture and ii) proxy-supervision attains state-of-theart for self-supervised monocular depth estimation


<div class="row" style="margin-top:7%">
    <img class="col-md-6" alt="architecture" style="max-width:100%;"  src="img/works/monoresmatch/architecture.png">
    <iframe class="col-md-6" style="max-width:100%;" width="100%" height="315" src="https://www.youtube.com/embed/h6Wo5MqbCY0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>


<div class="mx-auto" style="margin-bottom:-100px; margin-top:7%">
    <ul class="list-inline">
        <li>
            <a  style="color:#{{site.color.primary}};" href=" https://github.com/fabiotosi92/monoResMatch-Tensorflow" class="btn-social btn-outline"><i class="fa fa-2x fa-github"></i></a>
        </li>
        <li>
            <a  style="color:#{{site.color.primary}}; " href="https://arxiv.org/abs/1904.04144" class="btn-social btn-outline"><i class="fa fa-print fa-2x"></i></a>
        </li>
        <li>
            <a  style="color:#{{site.color.primary}};" data-dismiss="modal" class="btn-social btn-outline"><i class="fa fa-times fa-2x"></i></a>
        </li>
    </ul>
</div>
