---
layout: default
modal-id: 6
date: 2020-07-07
img: reversing.gif
alt: image-alt
project-date: July 2020
conference: European Conference on Computer Vision 2020
short: ECCV2020
keywords: [Stereo Matching -, Monocular Depth Estimation]  
title: Reversing the cycle&#58 self-supervised deep stereo through enhanced monocular distillation
authors: [F. Aleotti, F. Tosi, L. Zhang, M. Poggi and S. Mattoccia]
---

In many fields, self-supervised learning solutions are rapidly evolving and filling the gap with supervised approaches. This fact occurs for depth estimation based on either monocular or stereo, with the latter often providing a valid source of self-supervision for the former. 
In contrast, to soften typical stereo artefacts, we propose a novel self-supervised paradigm reversing the link between the two. Purposely, in order to train deep stereo networks, we distill knowledge through a monocular completion network. This architecture exploits single-image clues and few sparse points, sourced by traditional stereo algorithms, to estimate dense yet accurate disparity maps by means of a consensus mechanism over multiple estimations. 
We thoroughly evaluate with popular stereo datasets the impact of different supervisory signals showing how stereo networks trained with our paradigm outperform existing self-supervised frameworks. 
Finally, our proposal achieves notable generalization capabilities dealing with domain shift issues.

# Framework
Starting from a RGB stereo dataset, our goal is to train a robust deep stereo network. To obtain this result, we first generate sparse values using traditional stereo algorithms, then we train a Monocular Completion Network (MCN) to generate dense maps. This network is similar to a completion network, since it takes a single RGB image and a small subset of points from the all set of points provided by the traditional algorithm. We exploit the Consensus Mechanism over multiple predictions (leveraging random point extractions and augmentation techniques) to filter out uncertaint points from the maps predicted by MCN, obtaining our final maps (as in the banner gif). Finally, we train a deep stereo network using such maps. Even if we do not rely on active sensors or external informations than simple RGB stereo pairs, the resulting deep networks prove to be robust, even near occlusions, and reach state of the art performance. 

<div class="row" style="margin-top:7%">
    <img class="col-md-12" alt="architecture" style="max-width:100%;"  src="img/works/reversing/framework.jpg">
</div>

# Qualitative results

From top to bottom, the left, the right and the output of the self-supervised stereo network (PSMNet) trained with the monocular enhanced proxies.

<div class="row" style="margin-top:7%">
    <img class="col-md-12" alt="qualitative" style="max-width:100%;"  src="img/works/reversing/qualitative.jpg">
</div>

<div class="mx-auto" style="margin-bottom:-100px; margin-top:7%">
    <ul class="list-inline">
        <li>
            <a  style="color:#{{site.color.primary}};" href="https://github.com/FilippoAleotti/Reversing" class="btn-social btn-outline"><i class="fa fa-2x fa-github"></i></a>
        </li>
        <li>
            <a  style="color:#{{site.color.primary}}; " href="" class="btn-social btn-outline"><i class="fa fa-print fa-2x"></i></a>
        </li>
        <li>
            <a  style="color:#{{site.color.primary}};" data-dismiss="modal" class="btn-social btn-outline"><i class="fa fa-times fa-2x"></i></a>
        </li>
    </ul>
</div>
