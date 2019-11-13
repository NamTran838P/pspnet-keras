This repository contains a Keras implementation of Pyramid Scene Parsing Networks [PSPNet](https://github.com/hszhao/PSPNet) that works with the latest Python dependencies.  Citation for original paper and implementation:

@inproceedings{zhao2017pspnet,
  author = {Hengshuang Zhao and
            Jianping Shi and
            Xiaojuan Qi and
            Xiaogang Wang and
            Jiaya Jia},
  title = {Pyramid Scene Parsing Network},
  booktitle = {Proceedings of IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
  year = {2017}
}

To install: 

python setup.py install

Usage:
```
python3 pspnet.py
python3 pspnet.py -m pspnet101_cityscapes -i ../example_images/munster_000013_000019_leftImg8bit.png -o ../example_results/munster_000013_000019_leftImg8bit.png -s -f
python3 pspnet.py -m pspnet101_cityscapes -i $CITYSCAPES_DATASET/leftImg8bit/val -o $CITYSCAPES_RESULTS -s -ms -f
python3 pspnet.py -m pspnet101_voc2012 -i ../example_images/000129.jpg -o ../example_results/000129.png -s -f
python3 pspnet.py -m pspnet50_ade20k -i ../example_images/ADE_val_00000435.jpg -o ../example_results/ADE_val_00000435.png -s -f
python3 pspnet.py -m pspnet50_ade20k -i ../example_images/ade20k.jpg -o ../example_results/ade20k.png -s -f
```