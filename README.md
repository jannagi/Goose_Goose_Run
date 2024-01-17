# Goose Goose Run

## 게임 소개

---

**어느 대학의 마스코트로서의 삶에 질린 거위의 모험!**

기본적으로 플레이어(거위)가 동적으로 생성되는 다양한 지형에서 여러 장애물을 피하고, 아이템들을 활용하여 가능한 멀리 달리는 것을 목표로 하는 게임입니다.

달리는 속도가 게임이 진행될 수록 점점 빨라지기 때문에 색다른 속도감을 느낄 수 있습니다.

**장르: 2D 사이드 스크롤 러닝 액션**

**개발환경: Unity**

**플랫폼: Window / Android**

---


### 팀원

---

- **하준학** KAIST 전산학부 19학번  <a href="https://github.com/jannagi" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white"></a>
    
- **박은비** KAIST 전산학부 22학번  <a href="https://github.com/seoyuncho" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white"></a>
---



## 게임 특징

---

### 메인 화면

---

메인 화면에서는 게임 시작, 랭킹 보기, 게임 종료의 선택지가 주어진다.

---

### 게임 진행

---

목숨은 기본적으로 3개가 주어지고 아이템을 통해서 추가 목숨을 획득할 수 있다. 장애물에 부딪히면 목숨이 하나씩 차감되고 지형에서 떨어지면 목숨 개수에 관계없이 게임 오버가 된다.

---


### 아이템

---


**목숨 +1**


**무적 5초**


**부스터 4초**

---

### 그래픽

- asset strore의 무료 에셋인 sunnyland와 chatgpt가 생성하는 그림을 통하여 이미지 구성
- unity에서 제공하는 animation 기능을 통해 이미지를 연속적으로 배치하여 애니메이션 구현

### 애니메이션

- player에게 run, jump_up, jump_down, double jump, hurt 등의 애니메이션 구현
- OnAir, IsUp, Hurt, DoubleJump 등의 parameter를 만들어서 script에서 parameter 값을 변환해주어 player의 상태에 따라 애니메이션이 자연스럽게 전환되도록 구현
    

### 음향 효과 및 음악

- 앞서 언급한 sunnyland의 음악과 Freesound에서 음향을 다운받아 사용
- audiosource를 사용하여 script에서 audiosource 변수를 선언하고 적절한 타이밍에 audiosource를 플레이하도록 설정한 후 드래그 앤 드롭을 통해 변수 할당
    

### 맵 동적 생성

- 다양한 지형을 만들고 player가 일정 거리 내에 들어오면 랜덤으로 지형을 선택해 생성하고 player가 해당 지형을 완전히 지나가고 나면 사라지도록 함
    

---

- 참고 에셋
    
    Sunny Land: https://assetstore.unity.com/packages/2d/characters/sunny-land-103349
