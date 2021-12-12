Capstone-Design2

## 딥러닝 기반 Super resolution, Denoising 복합 모델 구현
Implement of Deep learning-based Super resolution, Denoising complex model

1. 연구 배경\
 최근 영상 서비스를 이용하는 사람들이 증가함에 따라 저화질의 이미지를 고화질로 변환하거나 영상 제공 서비스(YouTube, Netflix, etc.)에서 편의를 위해 영상을 압축한 뒤 고해상도의 디스플레이에서 제공하는 경우가 증가했다. 이에 따라 발생하는 Compression Noise를 제거함과 동시에 화질 개선 과정을 필요로 하게 되었다.
 따라서 본 연구에서는 Denoising과 Super Resolution 과정을 동시에 해결할 수 있는 모델의 사용 가능성을 확인하고자 한다.

2. 연구 목표\
 본 연구에서는 DnCNN("Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising (TIP, 2017)", https://github.com/cszn/DnCNN) 모델을 이용하여, Denoising과 Super Resolution을 동시에 진행하고자 하며, 이때의 loss function을 변경하여 Compression Noise를 제거할 때 어떤 방법이 가장 높은 성능을 보이는지 확인하고자 한다.
 
3. 사용 모델\
 DnCNN\
  ConV+ReLU, Conv+BN+ReLU, Conv로 이루어진 모델.
