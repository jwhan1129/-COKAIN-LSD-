
LSD
=================
## 1. Data preparation

Model을 구축하기 위해 인스타그램을 기반으로 Image crawling을 진행하였습니다.<br>
Crawling과정에서 Selenium library 기반으로 ChromeDriver를 이용하였으며, 인스타그램의 해시태그 및 인스타그램이 자동으로 제공하는 img.att의 하위 요소들을 활용하여 필터링하였습니다. 그 결과 총 2704개의 Training set과 588개의 test set을 구축할 수 있었습니다.
<br>
<br>
Crawling 된 img는 전처리 과정을 통해 학습 및 분석에 용이한 형태로 변형하였습니다. <br>



Learning은 크게 두 단계로 구성됩니다.

## 3. Service
