 OpenCV_With_MediaPipe
 ---
![스크린샷 2024-11-18 224640](https://github.com/user-attachments/assets/08884487-7cc7-49d1-b118-aab3e6098da9)

프로젝트 소개
---
OpenCV 와 MediaPipe를 사용하여 실시간 얼굴 인식 시스템을 사용해 얼굴 감지 후 이미지 오버레이를 통한 실시간 얼굴 꾸미기

프로젝트 전체 과정
----
![image](https://github.com/user-attachments/assets/12e0dd75-1082-49c2-aade-1c7be0fe1326)


주요 기능
---
● 이미지 투명도 처리 (make_white_transparent 함수) : 이미지를 입력받아 흰색 픽셀을 투명하게 변환하여 오버레이 이미지에 적합한 형식으로 만듬

● 오버레이 이미지 합성 : 주어진 좌표에 오버레이 이미지를 붙여 원본 이미지와 혼합. 알파 채널을 사용하여 투명도 조절

● 웹캠에서 실시간 이미지 캡처 : OpenCV의 VideoCapture를 사용하여 웹캠에서 실시간 비디오 스트림을 캡처하고, 얼굴 검출 작업 수행

● 얼굴 검출 및 특징점 인식 : MediaPipe의 얼굴 검출 모듈을 활용하여 얼굴과 주요 특징점(눈, 코 등)을 인식하고, 이를 오버레이 이미지의 위치로 사용

● 결과 출력 및 사용자 상호작용 : 합성된 이미지를 화면에 출력하며, 'q'키를 눌러 프로그램 종료

개발환경
---
● Jupyter Notebook : Google Colab에서는 웹캠 지원이 되지 않아 Jupyter Notebook을 사용해 실시간 비디오 스트림을 캡처하고 얼굴 검출 작업 수행

● Python : 주요 프로그래밍 언어로 사용

기술 스택
---
● OpenCV : 이미지 전처리 및 변환에 사용, 영상의 색상 변환, 오버레이 이미지 추가 등을 통해 실시간 얼굴 검출 및 시각화 작업 지원

● MediaPipe : 실시간 얼굴 검출 및 특징점 인식을 위한 라이브러리로, 사용자의 얼굴을 효과적으로 분석하고 시각화

● Numpy : 배열 및 행렬 연산을 위한 라이브러리로, 이미지 데이터 처리와 마스크 생성 작업에 사용

실시간 얼굴 꾸미기
---
![image](https://github.com/user-attachments/assets/e2ac70de-1740-4548-9ddc-a4b14889dba0)
