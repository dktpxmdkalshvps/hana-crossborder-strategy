# Data Sources

이 문서는 `Hana Cross-border Strategy` 프로젝트에서 실제로 활용한 원천데이터와 참고자료를 정리한 목록입니다.

분석에는 **공개 데이터, 공식 공시·IR 자료, 국제기구 보고서, 연구논문, 공개 기사**만 사용했습니다. 동일한 성격의 지표라도 정의·기간·측정 방식이 다를 수 있으므로, Tableau에서는 출처 간 숫자를 기계적으로 합치거나 단순 순위화하지 않고 각 자료의 역할과 비교 가능 범위를 구분했습니다.

## Source Policy

- **핵심 KPI 및 재무 수치**: 국제기구, 공식 공시, IR/Annual Report, 결산공고 등 1차 자료를 우선 사용
- **시장 구조 및 인과 해석**: IMF, BIS, FSB, 학술·기관 연구를 우선 사용
- **GIWA/GLN 및 최신 실행 사례**: 공식 공개자료와 복수의 공개 기사로 교차 확인
- **산업 블로그·해설 자료**: 기술 구조나 시장 Narrative의 보조 설명에 한정
- **PoC와 상용화 구분**: PoC, 공식 채택, Production 통합, Live 거래, 경제성을 서로 다른 단계로 취급
- **비교 가드레일**: 비용·속도·성숙도처럼 정의가 다른 지표는 동일 기준처럼 직접 랭킹하지 않음

> 링크는 원천데이터 목록 작성 시점의 공개 URL을 기준으로 합니다. 외부 사이트 개편에 따라 경로가 변경될 수 있습니다.

## 1. 시장·정책·연구
| 분류 | 자료 | 기간 / 기준일 | 출처 | Tableau 활용 |
|---|---|---|---|---|
| 송금시장 원천데이터 | [Remittance Prices Worldwide](https://datacatalog.worldbank.org/search/dataset/0037898/remittance-prices-worldwide) | 2011~2025, 분기 | World Bank | 377개 송금 corridor, 48개 송금국, 111개 수취국의 $200/$500 송금비용, FX margin, 사업자, 속도 등을 이용해 Global → Korea → Corridor 분석 |
| 송금비용 연구 | [What Explains Remittance Fees? Panel Evidence](https://www.imf.org/-/media/files/publications/wp/2022/english/wpiea2022063-print-pdf.pdf) | 2011~2020 중심 / 2022 발간 | IMF Working Paper WP/22/63 | Bilateral corridor별 송금비용 결정요인. 경쟁 사업자 수, 은행/MTO 구성, 인터넷 채널 등을 Cost Driver 분석에 활용 |
| 송금비용 연구 | [Understanding cost patterns in remittance corridors of sub-Saharan Africa](https://www.resbank.co.za/content/dam/sarb/what-we-do/payments-and-settlements/cross-border-payments-conference/documents/remittance-cost-patterns.pdf) | RPW 기반 / 2025 자료 | South African Reserve Bank | Corridor별 비용 편차, 은행·MTO 차이, 지역별 비용구조를 RPW 해석 보조근거로 활용 |
| Payment Rail 연구 | [Competing Rails for Cross-Border Payments: Banks, Fintechs, and Stablecoins](https://www.hbs.edu/ris/Publication%2520Files/Du_Huang_Scharfstein_14Feb2016_66992079-2e6b-4584-95cf-014441c77485.pdf) | 2026-02-15 | Wenxin Du, Catherine Huang, David Scharfstein — Harvard Business School | 은행/SWIFT, MTO, Stablecoin의 all-in cost를 동일 프레임으로 비교하고 Architecture·Cost·Liquidity·Speed·Regulation 차이를 분석 |
| 연구 해설 | [The Unfinished Reform of Global Payments](https://e-axes.com/the-unfinished-reform-of-global-payments/) | 2026-06-30 | e-axes | Cross-border payment 시장구조 및 Payment Rail 연구 해설. Rail 비교와 시장구조 해석의 보조자료 |
| 산업 참고 | [How Ripple and SWIFT Are Changing Global Payments](https://web3enabler.com/blog/how-ripple-and-swift-are-changing-global-payments/) | 2026-01-11 | Web3 Enabler | Ripple와 SWIFT의 기술·속도·네트워크 비교. 산업 Narrative 참고용 |
| 글로벌 인프라 | [Project Agorá and cross-border payments](https://flow.db.com/Topics/cash-management/project-agora-and-cross-border-payments) | 2024~2026 | Deutsche Bank flow | Tokenised commercial bank deposits와 central-bank reserves를 이용한 Agorá prototype 및 atomic settlement 분석 |
| 글로벌 인프라 | [BIS Project Agorá moves from blueprint to reality](https://paymentsindustryintelligence.com/bis-project-agora-moves-from-blueprint-to-reality/) | 2026 | Payments Industry Intelligence | Agorá의 blueprint → prototype/실행 단계 전환 해석 |
| 글로벌 인프라 | [Project mBridge reached minimum viable product stage](https://www.bis.org/about/bisih/topics/cbdc/mcbdc_bridge.htm) | 2022~2024+ | BIS Innovation Hub | Multi-CBDC 기반 실시간 cross-border payment 및 FX. Official-sector alternative rail 비교 |
| 글로벌 인프라 | [BIS Project Nexus Explained: What It Is, How It Works, 2027 Go-Live](https://www.paymentlabs.ai/project-nexus) | 2021~2027 계획 | Payment Labs | FPS를 신규 settlement asset 없이 연결하는 구조. Blockchain 외 대안의 Counterfactual로 활용 |
| 글로벌 결제 산업 | [Cross-border payments in 2026: Friction and reform](https://thepaymentsassociation.org/article/cross-border-payments-2026-friction-reform/) | 2026 | The Payments Association | Interoperability, ISO 20022, liquidity, FX, 규제 등의 friction 분석 |
| 통화·정책 | [Disruptions in the international monetary landscape: threats or promises?](https://www.banque-france.fr/en/governors-interventions/disruptions-international-monetary-landscape-threats-or-promises) | 2026 | Banque de France | Stablecoin·tokenisation, monetary sovereignty, 국제통화체계 분석 |
| 국제정책 KPI | [Annual Progress Report on Meeting the Targets for Cross-border Payments: 2024 Report on Key Performance Indicators](https://www.fsb.org/2024/10/annual-progress-report-on-meeting-the-targets-for-cross-border-payments-2024-report-on-key-performance-indicators/) | 2024 | Financial Stability Board | G20 Cross-border Payment Roadmap의 Cost·Speed·Access·Transparency KPI |
| 기존 은행망 연구 | [Pressures on Correspondent Banking: Impact, Drivers, and Responses](https://www.elibrary.imf.org/display/book/9781513523002/ch017.xml) | 2010년대 CBR 변화 | IMF | Correspondent banking 구조, de-risking, AML/CFT 비용, CBR 축소와 금융접근성 분석 |

## 2. 하나은행·GIWA·GLN
| 분류 | 자료 | 기간 / 기준일 | 출처 | Tableau 활용 |
|---|---|---|---|---|
| 하나 GIWA | [Hana Financial Completes Blockchain Remittance Test, Eyes Fee Revolution](https://en.sedaily.com/finance/2026/02/27/hana-financial-completes-blockchain-remittance-test-eyes) | 2026-02-27 | Seoul Economic Daily | GIWA 해외송금 PoC 완료, SWIFT messaging 대체, AML/KYC 테스트, deposit-token 계획 |
| 하나 GIWA | [Hana Financial Builds Blockchain Remittance Network to Replace SWIFT](https://en.sedaily.com/technology/2026/02/28/hana-financial-builds-blockchain-remittance-network-to) | 2026-02-28 | Seoul Economic Daily | GIWA PoC 및 향후 해외송금 인프라 구축 |
| 하나 GIWA | [두나무, 하나금융과 블록체인 기반 해외송금 길 텄다](https://news.bizwatch.co.kr/article/mobile/2026/02/27/0004) | 2026-02-27 | 비즈워치 | GIWA Chain, SWIFT 전문 대체, 하나·두나무 PoC 구조 |
| GLN | [Hana Bank Subsidiary GLN Expands QR Payment Network for International Travelers to Korea](https://www.newswire.ca/news-releases/hana-bank-subsidiary-gln-expands-qr-payment-network-for-international-travelers-to-korea-865100525.html) | 2026-08-01 | GLN International / Newswire | 국내 QR 약 150만, 글로벌 QR 2.3억+ 가맹점, 15개국 및 Usage 성장 |
| GLN 재무·사업 | [적자 늪 탈출 못한 GLN인터...향후 과제는](https://www.asiatoday.co.kr/kn/view.php?key=20240521010010658&utm) | 2024-05-01 | 아시아투데이 | GLN 영업수익·누적적자·순손실 구조. 공식 결산공고 교차검증용 |
| GLN 경쟁/개방성 | [케이뱅크, QR·바코드로 간편 결제…GLN 해외결제 서비스 출시](https://kr.investing.com/news/stock-market-news/article-1172933) | 2024 | 알파경제 / Investing.com 게재 | KBank 앱의 GLN 이용 사례. GLN의 open distribution infrastructure 성격 확인 |
| 하나 Legacy FX | ['외환 강자' 하나은행, 외환시장 24시간 거래에 선제적 대응체계 구축](https://marketin.edaily.co.kr/News/ReadE?newsId=02715846645511896&utm) | 2026 | 이데일리 Marketin | 24h FX 운영, FX Leading Bank, 현물환·FX Swap·전체 거래량 관련 공개 근거 |
| GLN 재무 원천 | [GLN International 결산공고](http://glninternational.com/) | 2021~2025 | GLN International | 자산·부채·자본·손익. GLN_FINANCIAL_2021_2025의 1차 원천 |
| 하나은행 재무 원천 | [하나은행 사업보고서](https://www.hanafn.com/ir/subMain.do) | 2021~2025 | DART / 하나은행 | 외화대출, 외화예수, 해외점포, 재무 및 사업정보 |
| 하나은행 재무 원천 | [하나은행 현황](https://www.hanafn.com/ir/subMain.do) | 2021~2025 | 하나은행 / 은행연합회 경영공시 | 외화자산총계·외화부채총계 등 4대은행 비교 |
| 하나금융 재무 원천 | [Hana Financial Group Annual Report](https://hanafn.com/en/ir/subMain.do) | 2021~2025 | Hana Financial Group | 글로벌 네트워크·해외사업·그룹 재무성과 |
| 하나금융 재무 원천 | [Hana Financial Group IR Databook](https://www.hanafn.com/en/ir/financial/databookDetail.do) | 2021~2025 | Hana Financial Group | FX 거래규모·점유율 및 그룹 KPI |

## 3. 국내 금융그룹 Benchmark
| 분류 | 자료 | 기간 / 기준일 | 출처 | Tableau 활용 |
|---|---|---|---|---|
| KB Benchmark | [KB국민은행 현황](https://www.kbfg.com/kor/ir/investor/list.jsp) | 2021~2025 | KB국민은행 | 외화자산·부채·대출·예수 데이터 |
| KB Benchmark | [KB Financial Group Fact Book](https://www.kbfg.com/eng/ir/report/factbook/list.jsp) | 2021~2025 | KB Financial Group | 그룹 사업·재무 KPI |
| KB Benchmark | [KB Financial Group Annual Report](https://www.kbfg.com/kor/ir/investor/list.jsp) | 2021~2025 | KB Financial Group | 해외사업·글로벌 전략·자회사 분석 |
| Shinhan Benchmark | [신한은행 현황](https://www.shinhan.com/hpe/index.jsp) | 2021~2025 | 신한은행 | 외화자산·부채·대출·예수 비교 |
| Shinhan Benchmark | [신한은행 사업보고서](https://dart.fss.or.kr/) | 2021~2025 | DART / 신한은행 | 재무·외화·해외법인 정보 |
| Shinhan Benchmark | [Shinhan Financial Group Annual Report](https://www.shinhangroup.com/en/ir/finance/annualReport) | 2021~2025 | Shinhan Financial Group | 글로벌 사업 및 전략 정보 |
| Woori Benchmark | [우리금융지주 현황(경영공시)](https://www.woorifg.com/) | 2021~2025 | 우리금융지주 | 우리은행 별도기준 외화자산·부채·대출·예수금 |
| Woori Benchmark | [Woori Financial Group Fact Book](https://www.woorifg.com/eng/investor/ir/fact-book/list.do) | 2021~2025 | Woori Financial Group | 그룹 및 은행 KPI 보조자료 |

## Data Lineage

원천자료는 `data/Hana_Decision_Intelligence_Tableau_Mart_v3_KR.xlsx`의 분석용 Mart로 정리한 뒤 Tableau에서 사용했습니다.

주요 분석 레이어는 다음과 같습니다.

- Remittance / Cross-border Market
- Cross-border Friction Taxonomy
- Payment Rail Benchmark
- Hana Legacy FX Execution
- GLN Network / Financial Data
- GIWA Digital Rail Roadmap
- 4대 금융그룹 Benchmark
- Claim / Evidence Registry
- Decision Matrix

## Reproducibility Notes

이 저장소는 공개용 포트폴리오 패키지입니다. 일부 원천자료는 외부 기관이 배포하는 PDF, IR 자료 또는 웹페이지이므로 원문 파일 전체를 저장소에 재배포하지 않고 **출처 링크와 가공 Mart**를 제공합니다.

외부 자료를 재수집할 경우에는 원문의 공표일·회계기간·단위·정의가 기존 Mart와 동일한지 확인한 뒤 사용해야 합니다.
