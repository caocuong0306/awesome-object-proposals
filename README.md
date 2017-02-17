# awesome-object-proposals [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of object proposals resources for object detection and deep learning.

## Table of Contents
- [Introduction](#introduction)
- [Tutorials](#tutorials)
- [Papers](#papers)
  - [Objectness Scoring](#objectness-scoring)
  - [Similarity Grouping](#similarity-grouping)
  - [Supervised](#supervised)
  - [Re-ranking & Post-processing](#re-ranking--post-processing)
  - [Evaluation](#evaluation)
- [Datasets](#datasets)
  
### Introduction
* [Generating Object Proposals] (https://pdollar.wordpress.com/2013/12/22/generating-object-proposals/) by Piotr Dollár.

### Tutorials

### Papers

#### Objectness Scoring
* Objectness [[Project]](http://groups.inf.ed.ac.uk/calvin/objectness/)
  * Bogdan Alexe, Thomas Deselaers, and Vittorio Ferrari, [What is an object?](http://groups.inf.ed.ac.uk/calvin/Publications/alexe-cvpr10.pdf), CVPR, 2010.
  * Bogdan Alexe, Thomas Deselaers, and Vittorio Ferrari, [Measuring the Objectness of Image Windows](https://www.vision.ee.ethz.ch/publications/papers/techreports/eth_biwi_00882.pdf), TPAMI, 2012.

#### Similarity Grouping
* CPMC [[Project]](http://home.isr.uc.pt/~joaoluis/cpmc/)
  * Joao Carreira and Cristian Sminchisescu, [Constrained Parametric Min-Cuts for Automatic Object Segmentation](http://home.isr.uc.pt/~joaoluis/papers/cvpr2010_2.pdf), CVPR, 2010.
  * Joao Carreira and Cristian Sminchisescu, [CPMC: Automatic Object Segmentation Using Constrained Parametric Min-Cuts](http://home.isr.uc.pt/~joaoluis/papers/PAMI2012.pdf), TPAMI, 2012.
* Endres [[Project]](http://vision.cs.illinois.edu/proposals/)
  * Ian Endres and Derek Hoiem, [Category Independent Object Proposals](http://link.springer.com/chapter/10.1007/978-3-642-15555-0_42), ECCV, 2010.
  * Ian Endres and Derek Hoiem, [Category-Independent Object Proposals With Diverse Ranking](http://dhoiem.cs.illinois.edu/publications/pami2013_proposals_endres.pdf), TPAMI, 2014.
* Selective Search [[Project]](http://koen.me/research/selectivesearch/)
  * Koen E. A. van de Sande, Jasper R. R. Uijlings, Theo Gevers, and Arnold W. M. Smeulders, [Segmentation As Selective Search for Object Recognition](http://koen.me/research/pub/vandesande-iccv2011.pdf), ICCV, 2011.
  * Jasper R. R. Uijlings, Koen E. A. van de Sande, Theo Gevers, and Arnold W. M. Smeulders, [Selective Search for Object Recognition](http://koen.me/research/pub/uijlings-ijcv2013-draft.pdf), IJCV, 2013.

#### Supervised

#### Re-ranking & Post-processing

#### Evaluation
* Boosting Object Proposals: From Pascal to COCO, ICCV, 2015 [[Paper]](http://www.vision.ee.ethz.ch/~biwiproposals/boosting-coco/data/PontTusetVanGool-Boosting-ICCV2015.pdf)[[Project]](http://www.vision.ee.ethz.ch/~biwiproposals/boosting-coco/index.html)
  * Jordi Pont-Tuset and Luc Van Gool. ETH Zürich.
* Object-Proposal Evaluation Protocol is 'Gameable', [[Paper]](https://arxiv.org/pdf/1505.05836.pdf)[[Project]](https://filebox.ece.vt.edu/~aroma/web/object-proposals.html)
  * Neelima Chavali, Harsh Agrawal, Aroma Mahendru, and Dhruv Batra. Virginia Tech.

### Datasets
* PASCAL [[Paper]](http://host.robots.ox.ac.uk/pascal/VOC/pubs/everingham10.pdf)[[Project]](http://host.robots.ox.ac.uk/pascal/VOC/)
  * Mark Everingham, Luc Van Gool, Christopher K. I. Williams, John Winn, and Andrew Zisserman, The PASCAL Visual Object Classes (VOC) Challenge, IJCV, 2010.
* MS COCO [[Paper]](https://arxiv.org/pdf/1405.0312.pdf)[[Project]](http://mscoco.org/)
  * Tsung-Yi Lin, Michael Maire, Serge Belongie, Lubomir Bourdev, Ross Girshick, James Hays, Pietro Perona, Deva Ramanan, C. Lawrence Zitnick, and Piotr Dollár, Microsoft COCO: Common Objects in Context, ECCV, 2014.
* ImageNet [[Paper]](http://www.image-net.org/papers/imagenet_cvpr09.pdf)[[Project]](http://www.image-net.org/)
  * Jia Deng, Wei Dong, Richard Socher, Li-Jia Li, Kai Li and Li Fei-Fei, ImageNet: A Large-Scale Hierarchical Image Database, CVPR, 2009.
* KITTI [[Paper]](http://www.cvlibs.net/publications/Geiger2012CVPR.pdf) [[Project]](http://www.cvlibs.net/datasets/kitti/index.php)
  * Andreas Geiger and Philip Lenz and Raquel Urtasun, Are we ready for Autonomous Driving? The KITTI Vision Benchmark Suite, CVPR, 2012.
