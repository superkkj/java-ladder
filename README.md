# 사다리 게임

## 1단계
### 기능 요구사항
- 사람 이름은 쉼표(,) 기준으로 구분
- 참여자 이름은 최대 5글자. 사다리 출력 시 이름도 같이 출력
- 사람 이름을 5자 기준으로 표시하기 때문에 사다리 폭도 이에 맞추어야 한다.
- 사다리 타기가 정상적으로 동작하려면 라인이 겹치지 않아야 한다.
  - `|-----|-----|` 이와 같이 가로가 겹치면 어디로 이동해야 할지 판단할 수 없다.
  
### 프로그래밍 요구사항
- 자바8의 람다와 스트림 적용
- 모든 엔티티를 작게 적용

### 실행 결과
- 4명의 사람이 참가하는 **5개 높이**의 사다리 만들 경우, 실행결과는 아래와 같다.


### 기능 분리
참가자 생성 
- Player
- [x] 이름이 null 이면 예외
- [x] 이름이 5자를 초과하면 예외

- Players
- [x] 참가자 리스트 생성(쉼표로 구분)
- [x] 참가자 명단이 null이면 예외
- [x] 참가자 명단이 2명 미만이면 예외

- Line
- [x] 사람 수만큼 생성된 사다리 사이의 라인이 한 라인에 중복되지 않아야 한다.

- Ladder
- [x] Line을 사다리 높이만큼 가진다.

# 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)