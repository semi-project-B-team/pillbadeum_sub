# pillbadeum_sub

필받음 백엔드·DB 준비 저장소임. 서버 코드·설정 예제·테스트·SQL은 `pillbadeum-server/`에 있음.

- [서버 실행](pillbadeum-server/README.md) · [DB 설치·갱신](pillbadeum-server/sql/README.md)
- 신규 DB: `00 → 01 → 13`이며 `02` 샘플 데이터는 선택임. `03~12`는 기존 DB 갱신용으로 보존함.
- 기존 DB: 이미 `11`까지 적용했다면 `12 → 13`을 적용함. 개인 DB에는 자동 적용하지 않음.
- [사진 등록 계약](pillbadeum-server/docs/PHOTO_REGISTRATION.md) · [낱알 식별 계약](pillbadeum-server/docs/PILL_IDENTIFICATION.md) · [OpenAPI JSON](pillbadeum-server/docs/openapi.json)
- 개인 `.env`, 실제 MySQL 데이터·Qdrant 볼륨은 공유하지 않음. 각 PC에서 준비하며 Qdrant는 `compose.qdrant.yaml`로 실행함.

로컬 Swagger는 서버 실행 후 `http://localhost:8080/swagger-ui/index.html`임. 최신 JSON은 실행 서버의 `/v3/api-docs`에서 받음.
