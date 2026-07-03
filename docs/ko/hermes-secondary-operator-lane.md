# Hermes 상호 보완 운영 Lane

## 요약

Hermes는 AI Engineering Lab에서 상호 보완 운영 lane으로 정리할 수 있다. 핵심은 OpenClaw가 넓은 조율과 승인 경계를 맡고, Hermes가 focused research, recovery review, follow-up automation, 공개 가능한 문서화를 별도 맥락에서 보조하는 역할이다.

다만 공개 표현은 조심해야 한다. Hermes를 무감독 자동 복구 agent로 말하지 않고, human approval gate 뒤에서 동작하는 complementary operator / audit-recovery lane으로 설명하는 것이 맞다.

## 공개 가능한 의미

- OpenClaw 같은 주 운영 assistant가 흔들릴 때 참고할 상호 보완 판단 경로
- 업데이트나 재시작 전 rollback과 smoke test를 다시 확인하는 독립 검토 lane
- private wiki의 운영 교훈을 public-safe 문서로 바꾸는 보조 경로
- focused research와 후속 자동화 후보를 별도 맥락에서 준비하는 경로
- 장시간 작업 중 context 손실이나 restart 이후에도 이어갈 수 있도록 돕는 운영 설계

## 계속 승인 뒤에 둘 작업

- 서비스 restart / stop / start
- OpenClaw 또는 Hermes config 변경
- package update 또는 version change
- credential, token, account 설정 처리
- GitHub release, portfolio live deploy, social posting

## 좋은 공개 문장

> Hermes를 상호 보완 운영 lane으로 구성해 OpenClaw 장애나 업데이트 위험 상황에서 audit, rollback review, recovery checklist 확인을 지원하도록 했다.

또는:

> OpenClaw와 Hermes를 상호 보완 operator lane으로 사용해 OpenClaw는 넓은 조율을 맡고, Hermes는 focused research와 recovery review를 맡도록 했다.

피해야 할 문장:

> Hermes가 OpenClaw를 자동으로 완전히 고치도록 만들었다.
