# 구현할 기능 정리

## 1
 - [] `구입금액을 입력해 주세요.` 라는 문구와 함께 로또 구입 금액을 입력 받는다.
  - [] 로또 구입 금액이 숫자가 아닐 경우, 예외를 발생시키고 다시 입력받는다.
   - `[ERROR] 올바른 형식의 숫자를 다시 입력해주세요.`
  - [] 로또 구입 가격이 음수일 경우, 예외를 발생시키고 다시 입력받는다.
   - `[ERROR] 0보다 큰 1000원 단위 숫자를 다시 입력해주세요.`
  - [] 로또 구입 가격이 1000으로 나누어 떨어지지 않을 경우, 예외를 발생시키고 다시 입력받는다.
   - `[ERROR] 0보다 큰 1000원 단위 숫자를 다시 입력해주세요.`

## 2
 - [] 로또를 발행한다.
  - [] 로또 번호는 오름차순으로 정렬한다.

## 3
 - [] 발행한 로또 수량 및 번호를 출력한다.
    ```
    8개를 구매했습니다.
    [8, 21, 23, 41, 42, 43]
    [3, 5, 11, 16, 32, 38]
    [7, 11, 16, 35, 36, 44]
    [1, 8, 11, 31, 41, 42]
    [13, 14, 16, 38, 42, 45]
    [7, 11, 30, 40, 42, 43]
    [2, 13, 22, 32, 38, 45]
    [1, 3, 5, 14, 22, 45]
    ```


## 4
 - [] 당첨 번호를 입력 받는다.
   - [] 로또 번호가 숫자 형식이 아닐 경우, throw문을 사용해 예외를 발생시키고 다시 입력받는다.
    - `[ERROR] 올바른 형식의 숫자를 다시 입력해주세요.`
   - [] 로또 번호가 1 ~ 45의 범위 안에 있지 않을 경우, throw문을 사용해 예외를 발생시키고 다시 입력받는다.
    - `[ERROR] 각 숫자를 1과 45 사이로 다시 입력해주세요.`
   - [] 로또 번호가 6개보다 적거나 많이 입력되면, throw문을 사용해 예외를 발생시키고 다시 입력받는다.
    - `[ERROR] 숫자가 6개인지 확인 후 다시 입력해주세요.`

## 5
 - [] 보너스 번호를 입력 받는다.
  - [] 보너스 번호가 숫자 형식이 아닐 경우, throw문을 사용해 예외를 발생시키고 다시 입력받는다.
    - `[ERROR] 올바른 형식의 숫자를 다시 입력해주세요.`
   - [] 보너스 번호가 1 ~ 45의 범위 안에 있지 않을 경우, throw문을 사용해 예외를 발생시키고 다시 입력받는다.
    - `[ERROR] 숫자를 1과 45 사이로 다시 입력해주세요.`
   - [] 보너스 번호가 1개보다 많이 입력되면, throw문을 사용해 예외를 발생시키고 다시 입력받는다.
    - `[ERROR] 숫자가 1개인지 확인 후 다시 입력해주세요.`
    
## 6
 - [] 당첨 내역을 출력한다.
    ```
    3개 일치 (5,000원) - 1개
    4개 일치 (50,000원) - 0개
    5개 일치 (1,500,000원) - 0개
    5개 일치, 보너스 볼 일치 (30,000,000원) - 0개
    6개 일치 (2,000,000,000원) - 0개
    ```

## 7
 - [] 수익률을 출력한다.
  - 수익률은 소수점 둘째 자리에서 반올림한다.
    ```
    총 수익률은 62.5%입니다.
    ```