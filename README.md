
LSD : Life Shot Director
=================
## 0. Intro

인스타그램의 발전과 함께 **사진**을 중심으로하는 SNS가 대세가 되어가고있습니다. <br>
하지만 인스타그램 인플루언서들처럼 좋은 사진을 찍는 것은 어려운 일입니다. <br>
Life Shot director(LSD)는 사진에 익숙하지 않은 사람도 언제 어디서나 최적의 구도로 사진을 찍을 수 있도록 가이드 라인을 제시합니다. <br>

LSD는 Naver Pose Estimation API와 다양한 Machine learning model을 활용하여 유저가 찍은 배경사진에서 학습된 패턴을 감지, 가장 많은 사람들이 위치했던 자리를 찾습니다. 

<br>
<div>
<img src= 'https://user-images.githubusercontent.com/61034754/74500390-14898900-4f2a-11ea-8317-f0d1f2f5559c.png', width = 1000>
<div>
<br>
최종적으로 저희는 위의 사진처럼 사진을 찍고자하는 배경을 찍으면, 유저가 가장 예쁜 사진을 찍기 위해 서야하는 위치와 개략적인 자세를 제시하고자 합니다. 


## 1. Data preparation
+ Image collecting<br>
Model을 구축하기 위해 인스타그램에서 Image crawling을 진행하였습니다.<br>
Crawling과정에서 Selenium library 기반으로 ChromeDriver를 이용하였으며, 인스타그램의 해시태그 및 인스타그램이 자동으로 제공하는 사진의 하위 요소들을 활용하여 필터링하였습니다. 그 결과 총 2704개의 Training set과 588개의 test set을 구축했습니다.
<br>
<div>
<img src= 'https://user-images.githubusercontent.com/61034754/74502473-f96e4780-4f30-11ea-8f0d-bff239b125b2.PNG', width = 1000>
<div>
<br>

+ Image pre-processing
Crawling 된 img는 전처리 과정을 통해 학습 및 분석에 용이한 형태로 변형하였습니다. <br>

<div>
<img src='https://user-images.githubusercontent.com/61034754/74502943-a5fcf900-4f32-11ea-8ddd-f850a5cda0ab.png', width = 1000>
<div>
<div>
<img src='https://user-images.githubusercontent.com/61034754/74502946-a7c6bc80-4f32-11ea-92f7-5cc41732c901.png', width = 1000>
<div>
## 2. Learning

Learning은 크게 두 단계로 구성됩니다.

## 3. Service





## 4. Citiation

**Deeplabv3+** : Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation, Liang-Chieh Chen and Yukun Zhu and George Papandreou and Florian Schroff and Hartwig Adam, ECCV, 2018 <br>

**DeepFill(inpainting)** : Generative Image Inpainting with Contextual Attention, Yu, Jiahui and Lin, Zhe and Yang, Jimei and Shen, Xiaohui and Lu, Xin and Huang, Thomas S, arXiv preprint arXiv:1801.07892, 2018 <br> yu2018free, Free-Form Image Inpainting with Gated Convolution, Yu, Jiahui and Lin, Zhe and Yang, Jimei and Shen, Xiaohui and Lu, Xin and Huang, Thomas S, arXiv preprint arXiv:1806.03589, 2018

**Holistically-nested edge detection (HED)** : Jia13caffe, Yangqing Jia, {Caffe}: An Open Source Convolutional Architecture for Fast Feature Embedding, 2013, http://caffe.berkeleyvision.org/ <br>
wu2016tensorpack, Tensorpack, Wu, Yuxin and others, https://github.com/tensorpack/, 2016

**VGG net** : simonyan2014deep, Very Deep Convolutional Networks for Large-Scale Image Recognition, Karen Simonyan and Andrew Zisserman, 2014, 1409.1556, arXiv, cs.CV
