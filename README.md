# 로또

---

## 프로젝트 개요

- 숫자 범위가 1~45인 로또를 발행한 뒤 번호를 추첨하여 당첨음 확인합니다.
- 사용자는 로또 구입 금액과 당첨 번호, 보너스 번호를 입력합니다.
    - 로또 구입 금액 만큼 장당 1,000원인 로또를 발행합니다.
    - 당첨 번호는 중복되지 않는 숫자 6개입니다.
    - 보너스 번호는 숫자 1개입니다.
- 발행한 로또는 중복되지 않는 무작위 6개의 숫자입니다.
- 당첨은 일치하는 숫자에 따라 1등부터 5등을 결정합니다.
- 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 출력합니다.

---

## 구현 기능 목록

- [x] **1. 입력 처리**
    - [x] 1-1. `로또 구입 금액`을 1,000원 단위로 하여 문자열로 입력받음
    - [x] 1-2. `당첨 번호`를 쉼표(,)를 기준으로 구분하여 문자열로 입력받음
    - [x] 1-3. `보너스 번호`를 분자열로 입력 받음

- [x] **2. 로또 수행**
    - [x] 2-1. 입력 받은 로또 구입 금액으로 구매한 로또 갯수 확인
    - [x] 2-2. 구매한 로또 수 만큼 로또 객체 생성
        - [x] 2-2-1. 1~45 사이의 중복되지 않는 무작위 수 생성
        - [x] 2-2-2. 로또 번호를 오름차순으로 정렬
    - [x] 2-3. 입력 받은 당첨 번호와 보너스 번호로 당첨 객체 생성

- [x] **3. 입력값 검증**
    - [x] 3-1. 입력한 모든 값이 숫자인지 검증
    - [x] 3-2. 로또 구입 금액이 1,000원으로 나누어 떨어지는지 검증
    - [x] 3-3. 당첨 번호의 구분자로 쉼표를 사용했는지 검증
    - [x] 3-4. 당첨 번호와 보너스 번호로 1~45의 숫자를 사용했는지 검증
    - [x] 3-5. 당첨 번호와 보너스 번호가 중복되는지 검증

- [x] **4. 당첨 확인**
    - [x] 4-1. 입력한 당첨 번호와 보너스 번호로 로또 당첨 확인

- [x] **5. 결과 출력 처리**
    - [x] 5-1. 당첨 기준에 따라 당첨된 수 출력
    - [x] 5-2. 총 수익률 출력
        - [x] 5-2-1. 소수점 둘째 자리에서 반올림

---