# awesome-object-proposals [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of object proposals resources for object detection.

=======
## Table of Contents
- [Introduction](#introduction)
- [Tutorials](#tutorials)
- [Papers](#papers)
  - [Objectness Scoring](#objectness-scoring)
  - [Similarity Grouping](#similarity-grouping)
  - [Supervised Learning](#supervised-learning)
  - [Hybrid & Part-based](#hybrid--part-based)
  - [RGB-D](#rgb-d)
  - [Re-ranking & Refinement](#re-ranking--refinement)
  - [Spatio-Temporal](#spatio-temporal)
  - [Low-Level Processing](#low-level-processing)
  - [Evaluation](#evaluation)
- [Datasets](#datasets)
- [Object Detection](#object-detection)

### Introduction
* [A Seismic Shift in Object Detection] (https://pdollar.wordpress.com/2013/12/10/a-seismic-shift-in-object-detection/) by Piotr Dollár.
* [Generating Object Proposals] (https://pdollar.wordpress.com/2013/12/22/generating-object-proposals/) by Piotr Dollár.

### Tutorials
* [ICCV 2015 Tutorial on Tools for Efficient Object Detection] (http://mp7.watson.ibm.com/ICCV2015/ObjectDetectionICCV2015.html)
  * Jan Hosang, [Region Proposals](http://mp7.watson.ibm.com/ICCV2015/slides/iccv_hosang.pdf).

### Papers

#### Objectness Scoring
  ![Objectness](https://c1.staticflickr.com/1/675/33118568516_bd088e181f_b.jpg)
* Objectness [[Project]](http://groups.inf.ed.ac.uk/calvin/objectness/)
  * Bogdan Alexe, Thomas Deselaers, and Vittorio Ferrari, [What is an object?](http://groups.inf.ed.ac.uk/calvin/Publications/alexe-cvpr10.pdf), CVPR, 2010.
  * Bogdan Alexe, Thomas Deselaers, and Vittorio Ferrari, [Measuring the Objectness of Image Windows](https://www.vision.ee.ethz.ch/publications/papers/techreports/eth_biwi_00882.pdf), TPAMI, 2012.
* Rahtu [[Project]](http://www.cse.oulu.fi/CMV/Downloads/ObjectDetection/)
  * Esa Rahtu, Juho Kannala, and Matthew Blaschko, [Learning a Category Independent Object Detection Cascade](http://www.ee.oulu.fi/~jkannala/publications/iccv2011.pdf), ICCV, 2011.
* Cascaded Ranking SVMs [[Code]](https://sites.google.com/a/brookes.ac.uk/zimingzhang/code)
  * Ziming Zhang, Jonathan Warrell, and Philip H. S. Torr, [Proposal generation for object detection using cascaded ranking SVMs](https://www.robots.ox.ac.uk/~tvg/publications/2011/ziming_cvpr11.pdf), CVPR, 2011.
* Salient
  * Jie Feng, Yichen Wei, Litian Tao, Chao Zhang, and Jian Sun, [Salient Object Detection by Composition](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6126348), ICCV, 2011.
* RandomizedSeeds
  * Michael Van den Bergh, Gemma Roig, Xavier Boix, Santiago Manen, Luc Van Gool, [Online Video SEEDS for Temporal Window Objectness](http://varcity.eu/paper/iccv2013_vandenbergh_videoseeds.pdf), ICCV, 2013.
* BING [[Project]](http://mmcheng.net/bing/)
  * Ming-Ming Cheng, Ziming Zhang, Wen-Yan Lin, and Philip Torr, [BING: Binarized Normed Gradients for Objectness Estimation at 300fps](http://mmcheng.net/mftp/Papers/ObjectnessBING.pdf), CVPR, 2014.
* CrackingBING
  * Qiyang Zhao, Zhibin Liu, Baolin Yin, [Cracking BING and Beyond](http://www.bmva.org/bmvc/2014/files/paper030.pdf), BMVC, 2014.
* BING++
  * Ziming Zhang, Yun Liu, Tolga Bolukbasi, Ming-Ming Cheng, and Venkatesh Saligrama, [BING++: A Fast High Quality Object Proposal Generator at 100fps](https://arxiv.org/pdf/1511.04511v1.pdf), arXiv:1511.04511.
  * Ziming Zhang, Xi Chen, Yanjun Zhu, Zhiguo Cao, Venkatesh Saligrama, and Philip H.S. Torr, [Sequential Optimization for Efficient High-Quality Object Proposal Generation](https://arxiv.org/pdf/1511.04511.pdf), arXiv:1511.04511v2.
* EdgeBoxes [[Project]](https://www.microsoft.com/en-us/research/publication/edge-boxes-locating-object-proposals-from-edges/) [[Code]](https://github.com/pdollar/edges)
  * Piotr Dollár and C. Lawrence Zitnick, [Edge Boxes: Locating Object Proposals from Edges](https://www.microsoft.com/en-us/research/wp-content/uploads/2014/09/ZitnickDollarECCV14edgeBoxes.pdf), ECCV, 2014.
* ContourBox
  * Cewu Lu , Shu Liu, Jiaya Jia and Chi-Keung Tang, [Contour Box: Rejecting Object Proposals Without Explicit Closed Contours](http://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Lu_Contour_Box_Rejecting_ICCV_2015_paper.pdf), ICCV, 2015.

#### Similarity Grouping
  ![SS](https://c2.staticflickr.com/4/3852/33003653872_6c034b1c93_o.jpg)
* CPMC [[Project]](http://home.isr.uc.pt/~joaoluis/cpmc/)
  * Joao Carreira and Cristian Sminchisescu, [Constrained Parametric Min-Cuts for Automatic Object Segmentation](http://home.isr.uc.pt/~joaoluis/papers/cvpr2010_2.pdf), CVPR, 2010.
  * Joao Carreira and Cristian Sminchisescu, [CPMC: Automatic Object Segmentation Using Constrained Parametric Min-Cuts](http://home.isr.uc.pt/~joaoluis/papers/PAMI2012.pdf), TPAMI, 2012.
* Endres [[Project]](http://vision.cs.illinois.edu/proposals/)
  * Ian Endres and Derek Hoiem, [Category Independent Object Proposals](http://link.springer.com/chapter/10.1007/978-3-642-15555-0_42), ECCV, 2010.
  * Ian Endres and Derek Hoiem, [Category-Independent Object Proposals With Diverse Ranking](http://dhoiem.cs.illinois.edu/publications/pami2013_proposals_endres.pdf), TPAMI, 2014.
* Selective Search [[Project]](http://koen.me/research/selectivesearch/)
  * Koen E. A. van de Sande, Jasper R. R. Uijlings, Theo Gevers, and Arnold W. M. Smeulders, [Segmentation As Selective Search for Object Recognition](http://koen.me/research/pub/vandesande-iccv2011.pdf), ICCV, 2011.
  * Jasper R. R. Uijlings, Koen E. A. van de Sande, Theo Gevers, and Arnold W. M. Smeulders, [Selective Search for Object Recognition](http://koen.me/research/pub/uijlings-ijcv2013-draft.pdf), IJCV, 2013.
* ObjSal [[Project]](http://www.iis.sinica.edu.tw/~liutyng/Projects/ObjSal/)
  * Kai-Yueh Chang, Tyng-Luh Liu, Hwann-Tzong, and Chen Shang-Hong Lai, [Fusing Generic Objectness and Visual Saliency for Salient Object Detection](http://www.iis.sinica.edu.tw/~liutyng/Publication_files/iccv11.pdf), ICCV, 2011.
* RandomizedPrim [[Project]](http://www.vision.ee.ethz.ch/~smanenfr/rp/index.html)
  * Santiago Manen, Matthieu Guillaumin, and Luc Van Gool, [Prime Object Proposals with Randomized Prim's Algorithm
](http://www.vision.ee.ethz.ch/~smanenfr/rp/ManenICCV2013.pdf), ICCV, 2013.
* Rantalankila
  * Pekka Rantalankila, Juho Kannala, and Esa Rahtu, [Generating Object Segmentation Proposals Using Global and Local Search
](https://users.aalto.fi/~kannalj1/publications/cvpr2014a.pdf), CVPR, 2014.
* RIGOR [[Project]](http://cpl.cc.gatech.edu/projects/RIGOR/)
  * Ahmad Humayun, Fuxin Li, and James M. Rehg, [RIGOR: Reusing Inference in Graph Cuts for Generating Object Regions](http://cpl.cc.gatech.edu/projects/RIGOR/pubs/humayun_CVPR_2014_rigor.pdf), CVPR, 2014.
* GOP [[Project]](http://www.philkr.net/2014/10/01/eccv/)
  * Philipp Krähenbühl and Vladlen Koltun, [Geodesic Object Proposals](http://www.philkr.net/papers/2014-10-01-eccv/2014-10-01-eccv.pdf), ECCV, 2014.
* MCG [[Project]](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/mcg/)
  * Pablo Arbelaez*, Jordi Pont-Tuset*, Jonathan T. Barron, Ferran Marques, Jitendra Malik, [Multiscale Combinatorial Grouping](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/mcg/resources/MCG_CVPR2014.pdf), CVPR, 2014.
  * Jordi Pont-Tuset*, Pablo Arbelaez*, Jonathan T. Barron, Ferran Marques, Jitendra Malik, [Multiscale Combinatorial Grouping for Image Segmentation and Object Proposal Generation](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/mcg/resources/MCG_arxiv2015_v3.pdf), TPAMI, 2017.

#### Supervised Learning
![RPN](https://c2.staticflickr.com/4/3821/33118567676_fecd47a78c_b.jpg)
* MultiBox [[Project]](https://github.com/google/multibox)
  * Dumitru Erhan, Christian Szegedy, Alexander Toshev, and Dragomir Anguelov, [Scalable Object Detection using Deep Neural Networks](https://arxiv.org/pdf/1312.2249.pdf), CVPR, 2014.
  * Christian Szegedy, Scott Reed, Dumitru Erhan, and Dragomir Anguelov, [Scalable, High-Quality Object Detection](https://arxiv.org/pdf/1412.1441.pdf), arXiv:1412.1441.
* DeepMask [[Code]](https://github.com/facebookresearch/deepmask)
  * Pedro O. Pinheiro, Ronan Collobert and Piotr Dollár, [Learning to Segment Object Candidates](https://arxiv.org/pdf/1506.06204.pdf), NIPS, 2015.
* Mid-level Cues
  * Tom Lee, Sanja Fidler, and Sven Dickinson, [Learning to Combine Mid-level Cues for Object Proposal Generation](http://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Lee_Learning_to_Combine_ICCV_2015_paper.pdf), ICCV, 2015.
* LPO [[Project]](http://vladlen.info/publications/learning-to-propose-objects/)
  * Philipp Krähenbühl and Vladlen Koltun, [Learning to Propose Objects](http://vladlen.info/papers/lpo.pdf), CVPR, 2015.
* RPN [[Project]](https://github.com/ShaoqingRen/faster_rcnn)
  * Shaoqing Ren, Kaiming He, Ross Girshick, and Jian Sun, [Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks](https://arxiv.org/pdf/1506.01497.pdf), NIPS, 2015.
* DeepProposal [[Code]](https://github.com/aghodrati/deepproposal)
  * Amir Ghodrati, Ali Diba, Marco Pedersoli, Tinne Tuytelaars, and Luc Van Gool, [DeepProposal: Hunting Objects by Cascading Deep Convolutional Layers](https://arxiv.org/pdf/1510.04445.pdf), ICCV, 2015.
* 3DOP [[Project]](http://www.cs.toronto.edu/objprop3d/)
  * Xiaozhi Chen, Kaustav Kundu, Yukun Zhu, Andrew Berneshawi, Huimin Ma, Sanja Fidler, and Raquel Urtasun, [3D Object Proposals for Accurate Object Class Detection](http://www.cs.toronto.edu/objprop3d/3dopNIPS15.pdf), NIPS, 2015.
* Mono3D [[Project]](http://3dimage.ee.tsinghua.edu.cn/cxz/mono3d)
  * Xiaozhi Chen, Kaustav Kundu, Ziyu Zhang, Huimin Ma, Sanja Fidler, and Raquel Urtasun, [Monocular 3D Object Detection for Autonomous Driving](http://3dimage.ee.tsinghua.edu.cn/files/publications/CVPR16_XiaozhiChen.pdf), CVPR, 2016.
* HyperNet
  * Tao Kong, Anbang Yao, Yurong Chen, and Fuchun Sun, [HyperNet: Towards Accurate Region Proposal Generation and Joint Object Detection](http://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Kong_HyperNet_Towards_Accurate_CVPR_2016_paper.pdf), CVPR, 2016.
* CRAFT [[Project]](https://github.com/byangderek/CRAFT)
  * Bin Yang, Junjie Yan, Zhen Lei, and Stan Z. Li, [CRAFT Objects From Images](https://arxiv.org/pdf/1604.03239.pdf), CVPR, 2016.
* AttractioNet [[Project]](https://github.com/gidariss/AttractioNet)
  * Spyros Gidaris and Nikos Komodakis, [Attend Refine Repeat: Active Box Proposal Generation via In-Out Localization](https://arxiv.org/pdf/1606.04446.pdf), BMVC, 2016.
* SPOP-net
  * Zequn Jie, Xiaodan Liang, Jiashi Feng, Wen Feng Lu, Eng Hock Francis Tay, and Shuicheng Yan, [Scale-Aware Pixelwise Object Proposal Networks](https://arxiv.org/pdf/1601.04798.pdf), TIP, 2016.
* FCN
  * Zequn Jie, Wen Feng Lu, Siavash Sakhavi, Yunchao Wei, Eng Hock Francis Tay, and Shuicheng Yan, [Object Proposal Generation with Fully Convolutional Networks](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7484700), TCSVT, 2016.
* InstanceFCN
  * Jifeng Dai, Kaiming He, Yi Li, Shaoqing Ren, and Jian Sun, [Instance-Sensitive Fully Convolutional Networks](https://arxiv.org/pdf/1603.08678.pdf), ECCV, 2016.
* MV3D [[Project]](http://3dimage.ee.tsinghua.edu.cn/cxz)
  * Xiaozhi Chen, Huimin Ma, Ji Wan, Bo Li, and Tian Xia, [Multi-View 3D Object Detection Network for Autonomous Driving](https://arxiv.org/pdf/1611.07759.pdf), arxiv.1611.07759. 2016.

#### Hybrid / Part-based
* ShapeSharing [[Project]](http://vision.cs.utexas.edu/projects/shapesharing/)
  * Jaechul Kim and Kristen Grauman, [Shape Sharing for Object Segmentation](http://www.cs.utexas.edu/~grauman/papers/shape-sharing-ECCV2012.pdf), ECCV, 2012.
* OOP [[Project]](http://www.shengfenghe.com/oriented-object-proposals.html)
  * Shengfeng He and Rynson W.H. Lau, [Oriented Object Proposals](http://www.shengfenghe.com/uploads/1/5/1/3/15132160/oop_iccv15.pdf), ICCV, 2015.
* Object Discovery [[Project]](http://www.di.ens.fr/willow/research/objectdiscovery/)
  * Minsu Cho, Suha Kwak, Cordelia Schmid, and Jean Ponce, [Unsupervised Object Discovery and Localization in the Wild: Part-based Matching with Bottom-up Region Proposals](http://www.di.ens.fr/willow/pdfscurrent/cho2015.pdf), CVPR, 2015.
* Adobe Boxes [[Code]](https://github.com/fzw310/AdobeBoxes-v1.0-/tree/master/AdobeBoxes(v1.0))
  * Authors, [Adobe Boxes: Locating Object Proposals Using Object Adobes](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7488218), TIP, 2016.

#### RGB-D
* MCG-D [[Project]](https://github.com/s-gupta/rcnn-depth)
  * Saurabh Gupta, Ross Girshick, Pablo Arbeláez and Jitendra Malik, [Learning Rich Features from RGB-D Images for Object Detection and Segmentation](https://people.eecs.berkeley.edu/~sgupta/pdf/rcnn-depth.pdf), ECCV, 2014.
* StereoObj [[Dataset]](http://www.cs.cityu.edu.hk/~rynson/papers/demos/StereoObj_Dataset.rar)
  * Shao Huang, Weiqiang Wang, Shengfeng He, and Rynson W.H. Lau, [Stereo Object Proposals​](http://www.cs.cityu.edu.hk/~rynson/papers/tip17.pdf), TIP, 2017.
* Elastic Edge Boxes
  * Jing Liu, Tongwei Ren, Yuantian Wang, Sheng-Hua Zhong, Jia Bei, Shengchao Chen, [Object proposal on RGB-D images via elastic edge boxes](http://www.sciencedirect.com/science/article/pii/S0925231216314266), Neurocomputing, 2017.

#### Re-ranking & Refinement
* MTSE [[Project]](http://3dimage.ee.tsinghua.edu.cn/cxz/mtse)
  * Xiaozhi Chen, Huimin Ma, Xiang Wang, Zhichen Zhao, [Improving Object Proposals with Multi-Thresholding Straddling Expansion](http://3dimage.ee.tsinghua.edu.cn/files/publications/CVPR15_XiaozhiChen.pdf), CVPR, 2015.
  * Xiaozhi Chen, Huimin Ma, Chenzhuo Zhu, Xiang Wang, Zhichen Zhao, [Boundary-aware box refinement for object proposal generation](http://3dimage.ee.tsinghua.edu.cn/download?filename=files/publications/NC17_XiaozhiChen.pdf), Neurocomputing, 2017.
* DeepBox [[Project]](https://github.com/weichengkuo/DeepBox)
  * Weicheng Kuo, Bharath Hariharan, and Jitendra Malik, [DeepBox: Learning Objectness with Convolutional Networks](https://arxiv.org/pdf/1505.02146.pdf), ICCV, 2015.
* SharpMask [[Code]](https://github.com/facebookresearch/deepmask)
  * Pedro O. Pinheiro, Tsung-Yi Lin, Ronan Collobert, and Piotr Dollár, [Learning to Refine Object Segments](https://arxiv.org/pdf/1603.08695.pdf), ECCV, 2016.
* DeepStereoOP
  * Cuong C. Pham and Jae Wook Jeon, [Robust Object Proposals Re-ranking for Object Detection in Autonomous Driving Using Convolutional Neural Networks](http://www.sciencedirect.com/science/article/pii/S0923596517300231), SPIC, 2017.

#### Spatio-Temporal
* STMOP [[Project]](https://www.cs.cmu.edu/~katef/videolearn.html)
  * Katerina Fragkiadaki, Pablo Arbelaez, Panna Felsen, and Jitendra Malik, [Learning to Segment Moving Objects in Videos](https://www.cs.cmu.edu/~katef/papers/CVPR2015_LearnVideoSegment.pdf), CVPR, 2015.

#### Evaluation
![Hosang](https://c1.staticflickr.com/1/721/33003654282_6b18185807_b.jpg)
* Hosang benchmark
 [[Project]](http://www.mpi-inf.mpg.de/departments/computer-vision-and-multimodal-computing/research/object-recognition-and-scene-understanding/how-good-are-detection-proposals-really/) [[Code]](https://github.com/hosang/detection-proposals)
  * Jan Hosang, Rodrigo Benenson, and Bernt Schiele, [How good are detection proposals, really?](https://arxiv.org/pdf/1406.6962.pdf), BMVC, 2014.
  * Jan Hosang, Rodrigo Benenson, Piotr Dollár, and Bernt Schiele, [What makes for effective detection proposals?](https://arxiv.org/pdf/1502.05082.pdf), TPAMI, 2016.
* Jordi Pont-Tuset and Luc Van Gool, [Boosting Object Proposals: From Pascal to COCO] (http://www.vision.ee.ethz.ch/~biwiproposals/boosting-coco/data/PontTusetVanGool-Boosting-ICCV2015.pdf), ICCV, 2015. [[Project]](http://www.vision.ee.ethz.ch/~biwiproposals/boosting-coco/index.html)
* Neelima Chavali, Harsh Agrawal, Aroma Mahendru, and Dhruv Batra, [Object-Proposal Evaluation Protocol is 'Gameable'] (https://arxiv.org/pdf/1505.05836.pdf), CVPR, 2016. [[Project]](https://filebox.ece.vt.edu/~aroma/web/object-proposals.html)

#### Low-Level Processing
![Low-level](https://c1.staticflickr.com/3/2939/33163181385_6386e3f029_z.jpg)
* Felzenszwalb's segmentation [[Project]](http://cs.brown.edu/~pff/segment/)
  * Pedro F. Felzenszwalb and Daniel P. Huttenlocher, [Efficient Graph-Based Image Segmentation](http://cs.brown.edu/~pff/papers/seg-ijcv.pdf), IJCV, 2004.
* SLIC [[Project]](http://ivrl.epfl.ch/research/superpixels)
  * Radhakrishna Achanta, Appu Shaji, Kevin Smith, Aurelien Lucchi, Pascal Fua, and Sabine Süsstrunk, [SLIC Superpixels Compared to State-of-the-art Superpixel Methods](https://infoscience.epfl.ch/record/177415/files/Superpixel_PAMI2011-2.pdf), TPAMI, 2012.
* Structured Edge Detection [[Code]](https://github.com/pdollar/edges)
  * Piotr Dollár and C. Lawrence Zitnick, [Structured Forests for Fast Edge Detection ](https://www.microsoft.com/en-us/research/wp-content/uploads/2013/12/DollarICCV13edges.pdf), ICCV, 2013.

### Datasets
  ![COCO](https://c2.staticflickr.com/4/3690/33003654372_bea4d16186_b.jpg)
* PASCAL [[Project]](http://host.robots.ox.ac.uk/pascal/VOC/)
  * Mark Everingham, Luc Van Gool, Christopher K. I. Williams, John Winn, and Andrew Zisserman, [The PASCAL Visual Object Classes (VOC) Challenge](http://host.robots.ox.ac.uk/pascal/VOC/pubs/everingham10.pdf), IJCV, 2010.
* MS COCO [[Project]](http://mscoco.org/)
  * Tsung-Yi Lin, Michael Maire, Serge Belongie, Lubomir Bourdev, Ross Girshick, James Hays, Pietro Perona, Deva Ramanan, C. Lawrence Zitnick, and Piotr Dollár, [Microsoft COCO: Common Objects in Context](https://arxiv.org/pdf/1405.0312.pdf), ECCV, 2014.
* ImageNet [[Project]](http://www.image-net.org/)
  * Jia Deng, Wei Dong, Richard Socher, Li-Jia Li, Kai Li and Li Fei-Fei, [ImageNet: A Large-Scale Hierarchical Image Database](http://www.image-net.org/papers/imagenet_cvpr09.pdf), CVPR, 2009.
* NYU Depth Dataset [[Project]](http://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html)
  * Nathan Silberman, Pushmeet Kohli, Derek Hoiem, and Rob Fergus, [Indoor Segmentation and Support Inference from RGBD Images](http://cs.nyu.edu/~silberman/papers/indoor_seg_support.pdf), ECCV, 2012.
* KITTI [[Project]](http://www.cvlibs.net/datasets/kitti/index.php)
  * Andreas Geiger and Philip Lenz and Raquel Urtasun, [Are we ready for Autonomous Driving? The KITTI Vision Benchmark Suite](http://www.cvlibs.net/publications/Geiger2012CVPR.pdf), CVPR, 2012.

#### Object Detection
  ![FastR-CNN](https://c1.staticflickr.com/1/715/32316133964_046a1c0f14_c.jpg)
* R-FCN [[Code]](https://github.com/daijifeng001/r-fcn)[[PyCode]](https://github.com/Orpine/py-R-FCN)
  * Jifeng Dai, Yi Li, Kaiming He, Jian Sun, [R-FCN: Object Detection via Region-based Fully Convolutional Networks](https://arxiv.org/pdf/1605.06409.pdf), NIPS, 2016.
* SSD [[Code]](https://github.com/weiliu89/caffe/tree/ssd)
  * Wei Liu, Dragomir Anguelov, Dumitru Erhan, Christian Szegedy, Scott Reed, Cheng-Yang Fu, Alexander C. Berg, [SSD: Single Shot MultiBox Detector](https://arxiv.org/pdf/1512.02325v2.pdf), ECCV, 2016.
* YOLO [[Code]](http://pjreddie.com/darknet/yolo/)
  * Joseph Redmon, Santosh Divvala, Ross Girshick, Ali Farhadi, [You Only Look Once: Unified, Real-Time Object Detection](http://pjreddie.com/media/files/papers/yolo.pdf), ECCV, 2016.
* Faster R-CNN [[Code]](https://github.com/ShaoqingRen/faster_rcnn) [[PyCode]] (https://github.com/rbgirshick/py-faster-rcnn)
  * Shaoqing Ren, Kaiming He, Ross Girshick, Jian Sun, [Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks](https://arxiv.org/pdf/1506.01497.pdf), NIPS, 2015.
* Fast R-CNN [[Code]](https://github.com/rbgirshick/fast-rcnn)
  * Ross Girshick, [Fast R-CNN](https://arxiv.org/pdf/1504.08083.pdf), ICCV, 2015.
* SPP [[Code]](https://github.com/ShaoqingRen/SPP_net)
  * Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun, [Spatial Pyramid Pooling in Deep Convolutional Networks for Visual Recognition](https://arxiv.org/pdf/1406.4729.pdf), ECCV, 2014.
* R-CNN [[Code]](https://github.com/rbgirshick/rcnn)
  * Ross Girshick, Jeff Donahue, Trevor Darrell, Jitendra Malik, [Rich feature hierarchies for accurate object detection and semantic segmentation](https://arxiv.org/pdf/1311.2524.pdf), CVPR, 2014.
