# Package Manifest

`hana-crossborder-strategy`는 사내 데이터 분석 경진대회 출품작을 외부에서도 검토할 수 있도록 정리한 공개용 GitHub 포트폴리오 패키지입니다.

## Package Contents

### Tableau
- `dashboard/hana_crossborder_strategy.twb`
- `dashboard/hana_crossborder_strategy.twbx`
- `dashboard/screenshots/` — 대시보드 5장 이미지

### Data
- `data/Hana_Decision_Intelligence_Tableau_Mart_v3_KR.xlsx`
  - Remittance / Cross-border Market
  - Cross-border Friction Taxonomy
  - Payment Rail Benchmark
  - Hana Legacy FX Execution
  - GLN Network / Financial Data
  - GIWA Digital Rail Roadmap
  - 국내 금융그룹 Benchmark
  - Claim / Evidence Registry
  - Decision Matrix

### Documentation
- `README.md` — 프로젝트 개요 및 대시보드 스토리
- `docs/data_sources.md` — 원천자료, 기간, 출처, 링크, 활용 목적
- `docs/methodology.md` — 분석 방법과 비교 가드레일
- `docs/publish_checklist.md` — 최종 공개 점검 및 선택 항목
- `data/README.md` — Mart 설명
- `dashboard/README.md` — Tableau 파일 설명
- `assets/README.md` — 대표 이미지 설명

### Presentation
- `presentation/hana_crossborder_strategy_overview.pptx`

## Source Scope

분석에는 회사 내부 데이터가 아닌 공개자료만 사용했습니다.

- World Bank RPW
- FSB Cross-border Payment KPI
- IMF / BIS / SARB 등 정책·연구자료
- Project Agorá / mBridge / Nexus 관련 공개자료
- 하나은행 Legacy FX 공개자료
- GIWA PoC 및 후속 공개자료
- GLN 네트워크·재무·사업 자료
- 하나·KB·신한·우리 금융그룹의 2021~2025 공시·IR 자료

원문 자료를 저장소에 일괄 재배포하지 않고, `docs/data_sources.md`에 출처와 링크를 기록하며 분석에 사용한 가공 데이터는 Tableau Mart로 제공합니다.

## Final Review Applied

이번 최종 패키지에서는 다음 사항을 정리했습니다.

- standalone `.twb`의 개인 PC 절대경로 제거
- `.twbx` 내부 Workbook / Data 파일명 정리
- 실제 저장소 파일명과 README / Manifest 일치
- 대시보드 스크린샷 5장 추가 및 README 연결
- 오래된 “파일 추가 예정” 문구 제거
- `dashboard/README.md` 및 `publish_checklist.md` 현행화
- 발표자료의 도구/로컬 사용자 메타데이터 제거
- 원천데이터 문서와 분석 범위 일치 여부 재검토

## Optional Links

GitHub Push 이후 필요에 따라 다음 링크만 추가하면 됩니다.

- Notion Portfolio
- Tableau Public
