# Sentential Logic

> proof는 수학의 핵심, deductive reasoning(연역적 추론) 은 proof의 기반

### Deductive reasoning

예를 들어

1. 내일은 비나 눈이 올 것이다. 눈이 오기에는 너무 따뜻하다. 그러므로 비가 올 것이다.
2. 만약 오늘이 일요일이라면 오늘은 일을 할 필요가 없다. 오늘은 일요일이다. 그러므로 나는 오늘 일을 할 필요가 없다.
3. 나는 오늘 아니면 내일 일한다. 나는 오늘 집에 있을 것이다. 그러므로 나는 내일 일할 것이다.

- premises(전제) 에서 conclusion(결론) 으로 이어지는 statements
- 예를 들어 3번 문항에서 "나는 오늘 아니면 내일 일한다." 와 "나는 오늘 집에 있을 것이다." 는 premises 이고 "그러므로 나는 내일 일할 것이다." 는 conclusion.
- conclusion이 true 라는 보장은 없다. conclusion은 premises중 하나라도 false 이어야만 false 가 될 수 있다. 모든 premise들이 true라면 conclusion 역시 true 일 것이다. 왜냐하면 premise들에 의해 conclusion이 결정되기 때문이다.
- argument가 올바르다고 말하려면 premises와 conclusion 사이에 인과가 있어야 한다. 다시 말해, premises가 전부 true일 때 conclusion이 false가 될 수 있다면 그 argument는 올바르지 않다.
---
$P$ or $Q$.

not $Q$.

Therefore, $P$.

---

argument의 주제가 무엇이든 간에 argument가 이런 형태를 취하고 있다면 argument는 올바르다고 말할 수 있다. statement가 아무리 복잡해도 상관없다.

- 이런 형태를 취함에 있어서 중요한 것은 "or", "not" 과 같은 단어들이다. statement를 **애매하지 않게** 결합할 수 있게끔 도와주기 때문이다.
- 그리고 이런 접속사들은 자주 사용되기 때문에 symbol로 나타내는데, 이를 connective symbols 라고 한다.

Symbol | Meaning
-------|---------
$\lor$ | or
$\land$| and
$\lnot$| not

즉, "P 혹은 Q" 라는 statement는 $P \lor Q$ 처럼 쓸 수 있고, "P 이면서 Q" 같은 statement는 $P \land Q$ 처럼 쓸 수 있다. 마찬가지로 "P가 아님" 은 $\lnot P$ 처럼 나타낼 수 있다.

이때 애매함을 없애기 위해 연산자 우선순위를 고려해야 할 수 있는데, 먼저 $\lnot$ 은 항상 바로 뒤에 오는 statement 에만 먼저 apply된다. 즉 $\lnot P \land Q$ 는 $(\lnot P) \land Q$ 이지, $\lnot (P \land Q)$ 가 아니다.

하지만 이 연산자들이 일상언어의 그것과 항상 대응되지는 않는다. "나와 너는 함께 있다" 라는 statement를 $나 \land 너$ 라고 표현할 수 없다는 말이다. 이 연산자들은 statement에만 적용될 수 있다.