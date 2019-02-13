# Mask R-CNN for Object Detection and Segmentation

### [Original version](https://github.com/matterport/Mask_RCNN)
### [Original paper](https://arxiv.org/pdf/1703.06870.pdf)

### Requirements
Create a new conda environment and install the following libraries. Don't forget to install jupyter notebook in the new environment to map tensorflow to it. Refer to https://github.com/tensorflow/tensorflow/issues/25507 for environment issue.
- python==3.5.5
- keras==2.1.3
- tensorflow-gpu==1.4.0
- tensorflow==1.4.0 (CPU only)
- cuda==8.0
- cudnn==6.0

### Train and test on my own data
- The corresponding [source code](https://github.com/shuuchen/Mask_RCNN/tree/master/samples/homes).

- Following this [tutorial](https://engineering.matterport.com/splash-of-color-instance-segmentation-with-mask-r-cnn-and-tensorflow-7c761e238b46), I create my own dataset with [VGG Image Annotator](http://www.robots.ox.ac.uk/~vgg/software/via/via.html). The labels are encoded and exported with a json file and decoded in HomesDataset class.

- Command lines for train and test

  ```
  # move to /path to Mask_RCNN/samples/homes
  python homes.py train --dataset ../../datasets/homes --weights coco
  ```
