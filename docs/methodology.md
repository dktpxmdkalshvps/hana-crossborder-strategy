# Methodology

## 1. 문제 정의

크로스보더 결제를 단순히 “블록체인이 빠른가”라는 기술 비교로 보지 않고, 실제 비용과 속도를 만드는 시장 구조·유동성·처리·규제·마지막 구간(last mile)까지 분해했습니다.

## 2. 분석 계층

분석은 다음 순서로 진행합니다.

1. **Market** — 실제 cross-border friction이 존재하는가
2. **Legacy** — 기존 FX·은행 결제망이 제공하는 기준선은 무엇인가
3. **Strategy** — 새로운 결제 레일이 해결하려는 문제는 무엇인가
4. **Execution** — PoC 또는 운영 수준의 실행 근거가 존재하는가
5. **Commercialization / Risk** — 반복 가능한 실거래·수익성·규제 대응이 확인되는가

## 3. 비교 원칙

비용, 속도, 성숙도, 네트워크 규모처럼 단위와 정의가 다른 지표를 하나의 종합점수로 합산하지 않습니다.

각 레일은 다음 기준을 분리해서 확인합니다.

- Architecture
- Settlement model
- FX / liquidity dependency
- Processing model
- Compliance model
- Interoperability
- Last-mile distribution
- Regulatory dependency
- Maturity / production evidence

## 4. Evidence Guardrails

- PoC와 production을 구분합니다.
- production과 commercialization을 구분합니다.
- 공개 근거가 없다는 사실을 실패의 증거로 해석하지 않습니다.
- 기술의 존재와 경제적 우위가 증명됐다는 주장을 분리합니다.
- GLN의 운영 네트워크와 GIWA의 디지털 rail 후보를 혼동하지 않습니다.

## 5. Tableau Story Design

### Dashboard 01 — Decision Readiness
Claim Registry의 정규화 상태, 선행조건, 차단 요인을 분리해 현재 근거가 어느 수준까지 판단 가능한지 보여줍니다.

### Dashboard 02 — Cross-border Friction & Rail Benchmark
시장 구조·FX·유동성·처리·컴플라이언스·상호운용성 등 마찰 요인을 분해한 뒤, Correspondent Banking, MTO, Stablecoin, Nexus, Agorá, mBridge, GIWA를 비교합니다.

### Dashboard 03 — Hana Position
GIWA와 분리해 기존 FX 실행 역량과 GLN 기반 유통 접점을 확인합니다.

### Dashboard 04 — GIWA Maturity
PoC, 후속 의향, 공식 채택, Production 통합, 성능 검증, Live 상용화, 경제성을 별도의 검증 단계로 관리합니다.

### Dashboard 05 — Strategic Decision
현재 확인된 근거와 미검증 영역, 그리고 어떤 추가 근거가 확보될 때 판단이 달라지는지를 Decision Matrix로 연결합니다.
