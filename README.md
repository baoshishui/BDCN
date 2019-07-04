## [Bi-Directional Cascade Network for Perceptual Edge Detection(BDCN)](https://arxiv.org/pdf/1902.10903.pdf)
## [Learning to Predict Crisp Boundaries(ECCV 2018)](http://openaccess.thecvf.com/content_ECCV_2018/papers/Ruoxi_Deng_Learning_to_Predict_ECCV_2018_paper.pdf)

This code is update the[code](https://github.com/pkuCactus/BDCN) into python3,and add the re_Dice loss which mentioned in Learning to Predict Crisp Boundaries(ECCV 2018).we apply it into face edge detection task,the experiment has achieved good results.

The first paper proposes a Bi-Directional Cascade Network for edge detection. By introducing a bi-directional cascade structure to enforce each layer to focus on a specific scale, BDCN trains each network layer with a layer-specific supervision. To enrich the multi-scale representations learned with a shallow network, we further introduce a Scale Enhancement
Module (SEM). Here are the code for this paper.

The second paper mainly proposed a useful loss to help the network learning a crisp edge .
## the experiment results
(left:the original results,right:add the re_Dice loss results)

<img src="demo/img1.png" width="100"> <img src="demo/img1_2.png" width="100">
<img src="demo/img2.png" width="100"><img src="demo/img2_2.png" width="100">
<img src="demo/img3.png" width="100"><img src="demo/img3_2.png" width="100">

### Prerequisites

- pytorch >= 0.2.0(Our code is based on the 0.2.0)
- numpy >= 1.11.0
- pillow >= 3.3.0
- python3

### Train and Evaluation

1. Clone this repository to local
```shell
git clone https://github.com/pytorch/pytorch.git
```

2. Download the imagenet pretrained vgg16 pytorch model [vgg16.pth](link: https://pan.baidu.com/s/10Tgjs7FiAYWjVyVgvEM0mA code: ab4g) or the caffemodel from the [model zoo](https://github.com/BVLC/caffe/wiki/Model-Zoo) and then transfer to pytorch version. You also can download our pretrained model for only evaluation.
The google drive [link](https://drive.google.com/file/d/1CmDMypSlLM6EAvOt5yjwUQ7O5w-xCm1n/view?usp=sharing).

3. Download the dataset to the local folder

4. running the training code train.py or test code test.py

### Pretrained models

BDCN model for BSDS500 dataset and NYUDv2 datset of RGB and depth are availavble on Baidu Disk.

    The link https://pan.baidu.com/s/18PcPQTASHKD1-fb1JTzIaQ
    code: j3de


The pretrained model will be updated soon.


