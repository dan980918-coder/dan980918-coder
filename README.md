# 오재민 | Data Analyst

데이터를 근거 기반으로 구조화하고, 실제 의사결정으로 연결하는 분석가입니다.

- 스포츠과학을 전공했고, 연구실에서 국가연구개발과제(e스포츠 시청 행태 분석, 기업 연계)의 API 데이터 수집·가공을 맡았습니다.
- K-Digital Training 데이터 분석 과정을 수료한 뒤, 이커머스 행동 로그 2.25억 건, 신용 이력 8개 테이블, 공공 API 62만 건을 SQL과 Python으로 직접 정리해 분석했습니다.
- 분석 결과를 타겟, 우선순위, 운영 기준처럼 현업이 바로 쓸 형태로 바꾸는 데 집중합니다.

![SQL](https://img.shields.io/badge/SQL-grey?style=flat-square) ![Python](https://img.shields.io/badge/Python-grey?style=flat-square) ![Pandas](https://img.shields.io/badge/Pandas-grey?style=flat-square) ![LightGBM](https://img.shields.io/badge/LightGBM-grey?style=flat-square) ![Tableau](https://img.shields.io/badge/Tableau-grey?style=flat-square) ![Streamlit](https://img.shields.io/badge/Streamlit-grey?style=flat-square) ![FastAPI](https://img.shields.io/badge/FastAPI-grey?style=flat-square) ![Docker](https://img.shields.io/badge/Docker-grey?style=flat-square) ![AWS](https://img.shields.io/badge/AWS-grey?style=flat-square)

## 대표 프로젝트

<table>
<tr>
<td width="280"><a href="https://github.com/dan980918-coder/crm-targeting-intelligence"><img src="https://raw.githubusercontent.com/dan980918-coder/crm-targeting-intelligence/main/reports/figures/12_buyer_path_breakdown.png" width="280"></a></td>
<td>

### [CRM 타겟팅 전략 설계](https://github.com/dan980918-coder/crm-targeting-intelligence)
개인 프로젝트, 2026.08~09

고객마다 다른 탐색·장바구니·구매 경로에 동일한 CRM 타기팅을 적용하는 게 맞는가. 고객 2,230만 명, 이벤트 2.25억 건의 행동 로그로 라이프사이클을 나누고 타겟팅 정책을 비교했다.

구매 유도 모델 AUC 0.865(규칙 기반 0.804), 동일 Recall 기준 접촉 인원 21.68~50.87% 절감. 재활성화는 모델이 규칙 기반 대비 우위가 없음을 확인해 규칙을 유지하기로 판단했다.

</td>
</tr>
<tr>
<td width="280"><a href="https://github.com/dan980918-coder/home-credit-default-risk"><img src="https://raw.githubusercontent.com/dan980918-coder/home-credit-default-risk/main/assets/figures/threshold_tradeoff.png" width="280"></a></td>
<td>

### [대출 채무불이행 예측](https://github.com/dan980918-coder/home-credit-default-risk)
팀(3명) 모델링 + 개인 확장, 2026.08~09

흩어진 신용 이력 8개 테이블(신청자 307,511명)로 대출 연체 가능성을 예측했다. 팀에서 모델링까지 진행한 뒤, 서빙·배포·모니터링·임계값 분석은 개인적으로 보완·확장했다.

Lean(A) + LightGBM 검증 AUC 0.7825(12개 조합 중 최고). 임계값 0.60에서 승인율 81.4%를 유지하며 승인군 연체율을 기저치의 절반 수준(4.6%)까지 낮추는 심사 기준을 제시했다.

</td>
</tr>
<tr>
<td width="280"><a href="https://github.com/dan980918-coder/road-incident-analysis"><img src="https://raw.githubusercontent.com/dan980918-coder/road-incident-analysis/main/outputs/figures/dashboard_screenshot.png" width="280"></a></td>
<td>

### [도로 돌발상황 분석](https://github.com/dan980918-coder/road-incident-analysis)
팀(3명), 2025.11~12

ITS 국가교통정보센터 돌발상황 데이터 62.3만 건으로 도로타입·시간대별 대응 우선순위를 찾았다. 도로타입·도로번호 기준 패턴 분석(H1, H4)을 담당했다.

도시고속국도는 교통사고 76.0%, 국가지원지방도는 공사 62.3%로 지배 유형이 정반대로 갈린다는 것을 카이제곱 검정과 Cramér's V로 확인했다(V=0.226, 중간 효과).

</td>
</tr>
</table>

## 분석하는 방식

| 단계 | 내용 |
|---|---|
| 문제 정의 | 분석 결과가 누구의 어떤 결정을 바꿀 것인지부터 명확히 한다 |
| 가설·지표 설계 | 검증 가능한 가설과 그걸 판단할 지표를 먼저 정한다 |
| 데이터 정리·품질 확인 | 결측·이상치·조인 무결성을 직접 확인하고 근거를 남긴다 |
| 의사결정 제안 | 수치를 운영 기준·타겟·우선순위처럼 바로 쓸 수 있는 형태로 바꾼다 |

## 경험

- **국가연구개발과제 · e스포츠 시청 행태 분석(기업 연계)**: API로 장시간 수집 시 40분~1시간마다 수집이 끊기는 문제를 30분 단위 CSV 분할 저장 방식으로 바꿔 데이터 손실 없이 수집을 완료했습니다.
- **성균관대학교 수업조교(2024.03~2025.03, 약 50명 수업)**: 채점 공지 회차당 평균 문의 11건이 들어오던 것을, 채점·안내 기준을 통일한 뒤 4~5건으로 줄였습니다.

## 학력 · 자격

- 성균관대학교 스포츠과학과 석사(2025.08), 학사(2024.02)
- K-Digital Training 데이터 분석 수료(2025.12, 프로그래머스)
- SQLD · ADsP · GAIQ · OPIc IM1

## 연락처

dan980918@gmail.com
