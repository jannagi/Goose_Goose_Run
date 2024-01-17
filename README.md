# Goose Goose Run

## 게임 소개

---

![스크린샷 2024-01-17 190639.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/698f1571-cfc1-41a8-a40e-0e7bbb7e6992/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_190639.png)

**어느 대학의 마스코트로서의 삶에 질린 거위의 모험!**

기본적으로 플레이어(거위)가 동적으로 생성되는 다양한 지형에서 여러 장애물을 피하고, 아이템들을 활용하여 가능한 멀리 달리는 것을 목표로 하는 게임입니다.

달리는 속도가 게임이 진행될 수록 점점 빨라지기 때문에 색다른 속도감을 느낄 수 있습니다.

**장르: 2D 사이드 스크롤 러닝 액션**

**개발환경: Unity**

**플랫폼: Window / Android**

---

## 게임 특징

---

### 메인 화면

---

메인 화면에서는 게임 시작, 랭킹 보기, 게임 종료의 선택지가 주어진다.

![스크린샷 2024-01-17 190639.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/698f1571-cfc1-41a8-a40e-0e7bbb7e6992/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_190639.png)

![스크린샷 2024-01-17 190939.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/6d4e79c9-d353-4125-94e1-00861238874d/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_190939.png)

---

### 게임 진행

---

목숨은 기본적으로 3개가 주어지고 아이템을 통해서 추가 목숨을 획득할 수 있다. 장애물에 부딪히면 목숨이 하나씩 차감되고 지형에서 떨어지면 목숨 개수에 관계없이 게임 오버가 된다.

![스크린샷 2024-01-17 191047.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/3a003a9d-659a-46ce-bbc5-437030bc3cb4/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_191047.png)

---

### 일시정지 화면

---

![스크린샷 2024-01-17 191209.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/8909f87b-34cc-400e-941b-9490d4617475/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_191209.png)

---

### 아이템

---

![**목숨 +1**](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/6884b92b-6450-4908-8fa9-05090a502dd6/%EB%AA%A9%EC%88%A8.png)

**목숨 +1**

![**무적 5초**](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/b069f422-925e-44de-9603-c855b22e8f8b/%EB%AC%B4%EC%A0%81.png)

**무적 5초**

![**부스터 4초**](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/b35940b1-50a1-4ea2-beca-3d1c7ec87757/%EB%B6%80%EC%8A%A4%ED%84%B0.png)

**부스터 4초**

---

### 그래픽

- asset strore의 무료 에셋인 sunnyland와 chatgpt가 생성하는 그림을 통하여 이미지 구성
- unity에서 제공하는 animation 기능을 통해 이미지를 연속적으로 배치하여 애니메이션 구현

### 애니메이션

- player에게 run, jump_up, jump_down, double jump, hurt 등의 애니메이션 구현
- OnAir, IsUp, Hurt, DoubleJump 등의 parameter를 만들어서 script에서 parameter 값을 변환해주어 player의 상태에 따라 애니메이션이 자연스럽게 전환되도록 구현
    
    ![스크린샷 2024-01-17 191451.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/a1cefd1e-ead5-4ac1-aca0-dba0a536df25/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_191451.png)
    

### 음향 효과 및 음악

- 앞서 언급한 sunnyland의 음악과 Freesound에서 음향을 다운받아 사용
- audiosource를 사용하여 script에서 audiosource 변수를 선언하고 적절한 타이밍에 audiosource를 플레이하도록 설정한 후 드래그 앤 드롭을 통해 변수 할당
    
    ![스크린샷 2024-01-17 191537.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/524dd5d6-e152-4a1e-8b96-16d9b6d7b130/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_191537.png)
    

### 맵 동적 생성

- 다양한 지형을 만들고 player가 일정 거리 내에 들어오면 랜덤으로 지형을 선택해 생성하고 player가 해당 지형을 완전히 지나가고 나면 사라지도록 함
    
    ![스크린샷 2024-01-17 191632.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/f6cb388f-3934-47d6-9928-26d2e10eb0fc/9f91763c-fd76-4a1e-9c5c-1ca97bbac030/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2024-01-17_191632.png)
    

---

- 참고 에셋
    
    Sunny Land: https://assetstore.unity.com/packages/2d/characters/sunny-land-103349
