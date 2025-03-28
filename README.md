# my_playful_cartoon
My little creation uses OpenCV magic to turn your image into a playful cartoon

# OpenCV를 활용한 만화 효과
이 프로젝트는 OpenCV를 사용하여 이미지를 만화 작품으로 변환하는 프로젝트입니다!

## 코드 개요
- **그레이스케일 변환**: 이미지를 흑백으로 변환하여 경계선을 감지합니다.
- **노이즈 제거**: 미디언 블러를 사용해 이미지를 부드럽게 처리합니다.
- **경계선 감지**: 적응형 임계값을 통해 경계선을 강조합니다.
- **색상 처리**: 이중 필터를 사용해 색상을 부드럽게 적용합니다.
- **만화 효과 결합**: 경계선과 색상을 결합해 최종 만화 스타일 이미지를 생성합니다.

## 데모 이미지

### 만화 효과가 잘 표현된 이미지
- 원래 이미지

![원래 이미지](/images/toys.jpg)

- 만화 이미지
  
![잘 표현된 이미지](/images/Cap%202025-03-23%2016-20-38-471.jpg)

### 만화 효과가 잘 표현되지 않은 이미지
- 원래 이미지

![원래 이미지](/images/my.jpg)

- 만화 이미지
  
![표현이 어려운 이미지](/images/Cap%202025-03-23%2016-39-55-020.jpg)

### 만화 효과가 잘 표현되는 이미지
- 선명한 경계선과 대비가 분명한 색상을 가진 사물 사진.
- 간단한 구조와 부드러운 표면, 뚜렷한 외곽선이 있는 사물 사진.

### 만화 효과가 잘 표현되지 않는 이미지
- 아주 자연스럽고 섬세한 풍경 이미지.
- 전체적인 색감이 비슷한 이미지나 색상의 대비가 부족한 이미지.

## 내 알고리즘의 한계점
1. 너무 많은 디테일과 복잡한 질감을 가진 이미지는 경계선이 흐려진다.
2. 흐릿한 외곽선 및 대비감 없는 색상은 감지가 어렵다.
3. bilateralFilter와 같은 함수는 계산 비용이 높아 고해상도 이미지를 처리하는 경우 속도가 느리다.
4. 이 알고리즘은 이미지의 스타일에 따른 세밀한 제어는 불가능(예: 특정 영역 강조, 색상 조정 등).


