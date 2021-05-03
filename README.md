# TDDPractice
TDD를 해보자!

이메일 입력 기능을 담은 앱 TDD

ref. https://medium.com/@nongdenchet/test-driven-development-with-mvvm-in-android-bcfad84e34e3

# 테스팅?
구현, 설계 과정에서 실수를 잡아내는 것

코딩, 설계 = 창조 / 테스팅 = 파괴
## 목적
- 요구사항과 일치하는 제품임을 확인
- 사용자가 제품을 사용하는 동안 crash가 일어나지 않도록
- 개발 단계에서 발생하는 결함과 오류를 찾아냄
## 테스트코드 효과
- 다양한 예외상황을 직접 만들어 테스트(더미 데이터, 다양한 인풋 값을 코드로 생성 및 사용)
- 기능 추가 및 수정 이후 잘 짜여진 테스트코드를 실행함으로써 부작용을 줄이고 마음 편하게 코딩!
- 실패한 테스트케이스를 통해 오류의 위치를 더 쉽고 빠르게 찾고 수정
- 빠른 테스트
- 문서로서의 역할
# TDD
Test Driven Development, 테스트코드를 개발 전에 먼저 작성하는 개발 방식
## vs. 프로덕선 코드 작성 뒤 테크스 코드 작성
- 테스트코드를 먼저 작성하고 그에 맞춰 프로덕션 코드를 짜기 때문에 자연스럽게 testable한 코드 작성
- 명세를 보고 나올 수 있는 성공/실패 케이스를 예측, 테스트 코드 작성
(작성된 프로덕션 코드를 읽고 끼워 맞춰 테스트코드를 만들었기 때문에 테스트코드를 통과함. 실패 케이스를 떠올리기 어려울 수 있음)
## TDD cicle of life
![image](https://user-images.githubusercontent.com/31833972/116834863-f5dce400-abfa-11eb-8657-72ec02955ae7.png)

- 실패하는 테스트케이스를 작성한다 (Red)
- 테스트를 통과하는 로직을 구현한다 (Green)
- 구현한 코드를 리팩토링한다 (Refactor)

모든 요구조건을 만족할 때까지 위 짧은 개발 cycle을 반복한다
## 장점
- 위 사이클을 따르며 한가지 일에만 집중할 수 있음(내가 지금 무엇을 해야하는지 분명히 정의하고 개발)
- 테스트 용이한 프로덕션 코드 작성
- 코드의 재사용성 증가
- 어려운 일을 작은 단계로 쪼갤 수 있음
- 더 다양한 예외상황을 뽑아낼 수 있고, 크리티컬한 예외 상황이 생길 확률이 낮아짐

👉 소프트웨어가 점점 커지고 복잡해지기 시작해도, TDD의 장점으로 인해 쉽고 편하게 개발할 수 있을 것
## 단점
간단한 개발 시, 오히려 생산성을 저하 시킬 수 있음
