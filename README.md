# spring-gift-point

## 포인트 적립/결제 서비스

1. 회원가입시 3000 포인트를 지급한다.
2. 포인트는 주문할 때 결제 금액에서 차감하여 사용할 수 있다.
    - 단, 포인트는 결제 금액의 총액 50%를 넘지 않아야 한다.
3. 사용자는 구매한, 즉 주문한 상품 금액의 5%를 포인트로 돌려 받게 된다.

## 기능 명세서

### Order

- 사용한 포인트, 남은 포인트, 적립 포인트 필드를 추가한다.
- 결제 금액에서 포인트를 차감한다.
    - 포인트는 결제 금액의 총액 50%를 넘지 않아야 한다.
    - 포인트가 부족하면 결제가 불가능하다.
    - 결제금액보다 큰 포인트를 사용할 수 없다.
- 주문 금액의 5%를 포인트로 적립한다.

### User

- 회원가입시 3000 포인트를 지급한다.
- 사용자의 포인트를 조회할 수 있다.