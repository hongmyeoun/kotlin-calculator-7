# 1주차 문자열 덧셈 계산기

## 기능 요구 사항
입력한 문자열에서 숫자를 추출하여 더하는 계산기를 구현한다.

- 쉼표(,) 또는 콜론(:)을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환한다.
```
예: "" => 0, "1,2" => 3, "1,2,3" => 6, "1,2:3" => 6
```
- 앞의 기본 구분자(쉼표, 콜론) 외에 커스텀 구분자를 지정할 수 있다. 커스텀 구분자는 문자열 앞부분의 "//"와 "\n" 사이에 위치하는 문자를 커스텀 구분자로 사용한다.
```
예: "//;\n1;2;3" => 6
```
- 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.

### 실행 결과 예시
```declarative
덧셈할 문자열을 입력해 주세요.
1,2:3
결과 : 6
```
## 기능 목록

### 입력
  - [X] ~~입력 메세지~~
  - [ ] 커스텀 구분자 확인
    - [ ] "//"와 "\n"사이의 문자
  - [X] ~~구분자 확인~~
    - [X] ~~쉼표(,)~~
    - [X] ~~콜론(:)~~

### 출력
  - [X] ~~결과 : 구분자를 기준으로 분리된 각 숫자의 합~~
  
### 오류처리
  - [ ] 입력이 잘못될 경우
    - [ ] 문자열이 입력되지 않은 경우 
    - [ ] 숫자가 양수가 아닌 경우
    - [ ] case 1) 커스텀 구분자가 없을 경우
      - [ ] 입력된 문자열에 숫자와 쉼표(,), 콜론(:)을 제외한 다른 문자가 있을 경우
    - [ ] case 2) 커스텀 구분자가 있을 경우
      - [ ] 커스텀 구분자와 숫자, 쉼표, 콜론을 제외한 다른 문자가 있을 경우
    
### 테스트
  - [ ] 오류처리들에 관한 내용
  - [ ] 예상되는 결과