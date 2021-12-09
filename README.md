<<<<<<< Updated upstream
# PitchDetection
=======
# PitchDetection

# **🎯Certune🎵**

> 음성 인식 기반 사용자 음정 교정 서비스



### 유튜브 채널





### 프로젝트 목적

자신의 음역대를 알지 못해 다양한 상황에서 노래를 부르기 어려워하는 사람들이 많지만, 이를 혼자서 개선하기는 어렵습니다. 대면 레슨의 경우, 시간과 비용이 많이 들며 유튜브 영상은 사용자의 음성에 대한 피드백이 없는 일방향성 학습이므로 음감을 교정하기는 어렵습니다.

따라서 저희는 사용자의 음성에 대한 정확한 피드백과 취약 소절에 대한 연습, 그리고 음감 향상을 위해 음성 인식 기반 사용자 음정 교정 서비스(이하, 'Certune')을 제안하게 되었습니다.  



### 주요 기능

- **회원 가입**

- **음정 테스트** 

- **음악 추천**(인기순/이름순/마이뮤직)

- **노래 연습**

  - 노래의 제목과 가사 표시

  - 난이도 표시
  - 자동 키 조절 모드

- **결과 확인**

  - 사용자의 점수 표시

  - 한 줄 피드백(고음/저음/박자/크기)

  - 연습이 필요한 소절 추출

- **나의 기록 확인**

  - 지금까지 부른 노래를 점수와 함께 확인.
  - 노래 연습에서 추출한 취약 소절을 노래별로 확인
  - 소절별로 원래 음원 재생 및 사용자의 음성을 재녹음

- **음감 교정**

  - 박자 교정

  - 음정 교정



### 시나리오

1. 어플리케이션에 접속, 음정 테스트 진행

2. 자신의 음역대 확인

3. 원하는 기능 선택

   **A. 노래 연습 및 피드백 확인**

   1. 노래 부르기 탭에서 원하는 노래 선택
   2. 해당 노래의 난이도 확인 및 자동 키 조절 옵션 선택
   3. 노래 부르기
   4. 자신의 점수와 문장 피드백 확인
   5. 연습이 필요한 소절 들어보기

   **B. 취약 소절 다시 녹음**

   1. 마이 레코드 탭 선택
   2. 노래별로 묶여있는 취약 소절과 각 노래의 점수 및 피드백 확인
   3. 연습을 원하는 노래 선택
   4. 취약 소절에 대한 원곡 청취 및 음성 재녹음

   **C. 음감 교정**

   1. 박자 교정을 하기 위해 여러가지 박자 중 하나를 선택하여 따라 부름
   2. 녹음된 내용을 듣고 다시 연습
   3. 음정 교정을 하기 위해 옥타브별 표준 음정을 따라 부름
   4. 녹음된 내용을 듣고 다시 연습



### 프로젝트 아키텍쳐

------

![](C:\Users\Kang Minji\Downloads\캡처.PNG)



### To-Do List

1. 실시간 사용자 음성 인식(pitch detection) ✅

2. 사용자의 음성 및 노래 음원에서 음정 및 박자 추출(TarsosDSP) ✅

3. 사용자의 음역대에 따라 기존 음원의 키 조정(pitch shifting)
4. 사용자의 음성만 인식할 수 있도록 민감도 조정

5. 음원 및 MR을 소절별로 분리

6. 노래 추천 기능 알고리즘 작성

7. 사용자 음성과 기존 음원 정확도 추출 : 사용자 음성의 {시간 : 음정}과 기존 음원의 {시간 : 음정}을 비교하여 정확한 시간에 정확한 음을 불렀는지 확인하는 알고리즘을 작성

8. 정확도에 따른 피드백 문장 작성 : 음정, 박자, 크기 3요소를 기준으로 피드백을 작성

9. 앱 뷰 개발



### 참고 자료

- TarsosDSP 라이브러리

  https://github.com/JorenSix/TarsosDSP
>>>>>>> Stashed changes
