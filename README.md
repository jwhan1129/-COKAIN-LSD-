
LSD : Life Shot Director
=================
## 0. Intro

Life Shot director(LSD)는 언제 어디서나 유저에게 최적의 사진 구도를 제시하는 app입니다. <br>
LSD은 유저가 배경사진을 찍으면, 
<br>
<div>
<img src= 'https://user-images.githubusercontent.com/61034754/74499342-b60edb80-4f26-11ea-8cba-99542d5613cd.png', width = 400>
<img src= 'https://user-images.githubusercontent.com/61034754/74499344-b6a77200-4f26-11ea-9efe-18c037235166.png' , width = 400>
<div>


## 1. Data preparation

Model을 구축하기 위해 인스타그램을 기반으로 Image crawling을 진행하였습니다.<br>
Crawling과정에서 Selenium library 기반으로 ChromeDriver를 이용하였으며, 인스타그램의 해시태그 및 인스타그램이 자동으로 제공하는 img.att의 하위 요소들을 활용하여 필터링하였습니다. 그 결과 총 2704개의 Training set과 588개의 test set을 구축할 수 있었습니다.
<br>
<br>
Crawling 된 img는 전처리 과정을 통해 학습 및 분석에 용이한 형태로 변형하였습니다. <br>



Learning은 크게 두 단계로 구성됩니다.

## 3. Service





## 4. Citiation

**Deeplabv3+** : Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation, Liang-Chieh Chen and Yukun Zhu and George Papandreou and Florian Schroff and Hartwig Adam, ECCV, 2018 <br>

**DeepFill(inpainting)** : Generative Image Inpainting with Contextual Attention, Yu, Jiahui and Lin, Zhe and Yang, Jimei and Shen, Xiaohui and Lu, Xin and Huang, Thomas S, arXiv preprint arXiv:1801.07892, 2018 <br> yu2018free, Free-Form Image Inpainting with Gated Convolution, Yu, Jiahui and Lin, Zhe and Yang, Jimei and Shen, Xiaohui and Lu, Xin and Huang, Thomas S, arXiv preprint arXiv:1806.03589, 2018

**Holistically-nested edge detection (HED)** : Jia13caffe, Yangqing Jia, {Caffe}: An Open Source Convolutional Architecture for Fast Feature Embedding, 2013, http://caffe.berkeleyvision.org/ <br>
wu2016tensorpack, Tensorpack, Wu, Yuxin and others, https://github.com/tensorpack/, 2016

**VGG net** : simonyan2014deep, Very Deep Convolutional Networks for Large-Scale Image Recognition, Karen Simonyan and Andrew Zisserman, 2014, 1409.1556, arXiv, cs.CV
