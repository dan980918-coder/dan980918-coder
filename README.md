# 오재민 | Data Analyst

데이터로 현업의 판단 기준을 만듭니다. 누구의 대출을 승인할지, 누구에게 메시지를 보낼지, 어느 도로에 무엇을 대비할지처럼 매일 반복되는 결정에 숫자로 된 기준을 세우는 일을 해왔습니다.

스포츠과학을 전공했고, 연구실에서 국가연구개발과제(e스포츠 시청 행태 분석, 기업 연계)의 API 데이터 수집·가공을 맡으며 데이터 분석으로 방향을 정했습니다. 코드는 AI(Claude Code)와 함께 작성하고, 문제 정의·가설·판정 기준·결과 검토는 직접 합니다.

![SQL](https://img.shields.io/badge/SQL-grey?style=flat-square) ![DuckDB](https://img.shields.io/badge/DuckDB-grey?style=flat-square) ![Python](https://img.shields.io/badge/Python-grey?style=flat-square) ![pandas](https://img.shields.io/badge/pandas-grey?style=flat-square) ![LightGBM](https://img.shields.io/badge/LightGBM-grey?style=flat-square) ![scikit--learn](https://img.shields.io/badge/scikit--learn-grey?style=flat-square) ![Tableau](https://img.shields.io/badge/Tableau-grey?style=flat-square)

## 대표 프로젝트

<table>
<tr>
<td width="280"><a href="https://github.com/dan980918-coder/crm-purchase-signal-targeting"><img src="https://raw.githubusercontent.com/dan980918-coder/crm-purchase-signal-targeting/main/v2/docs/figures/capture_curve.png" width="280"></a></td>
<td>

### [구매 신호 기반 CRM 발송 대상 선정 기준 설계](https://github.com/dan980918-coder/crm-purchase-signal-targeting)
개인 프로젝트, 2026.08~10

한정된 CRM 발송량을 누구에게 먼저 쓸 것인가. 발송 상위 10% 기준으로 구매 고객 포착률을 최근 활동 순 35%에서 76%로 높여, 발송 1만 건당 구매 고객이 320명에서 691명으로 늘어난다. 같은 수의 구매 고객을 발송량 86% 적게 잡을 수 있다.

</td>
</tr>
<tr>
<td width="280"><a href="https://github.com/dan980918-coder/loan-approval-risk-scoring"><img src="https://raw.githubusercontent.com/dan980918-coder/loan-approval-risk-scoring/main/v2/docs/figures/tradeoff_champion_vs_challenger.png" width="280"></a></td>
<td>

### [연체 위험 기반 대출 승인 기준 설계](https://github.com/dan980918-coder/loan-approval-risk-scoring)
팀(3명) + 개인 재설계, 2026.08~10

승인율을 지키면서 연체할 고객만 골라낼 수 있는가. 승인율 80%로 심사하면 승인 고객 연체율이 8.1%에서 4.6%로 떨어진다. 외부 신용점수만 쓸 때(5.3%)보다 12% 낮은 수준이고, 같은 연체율이면 승인을 6%p 더 늘릴 수 있다.

</td>
</tr>
<tr>
<td width="280"><a href="https://github.com/dan980918-coder/road-incident-response-planning"><img src="https://raw.githubusercontent.com/dan980918-coder/road-incident-response-planning/main/outputs/figures/dashboard_screenshot.png" width="280"></a></td>
<td>

### [돌발 유형 기반 도로 대응 기준 설계](https://github.com/dan980918-coder/road-incident-response-planning)
팀(3명), 2025.11~12

도로 종류·노선·시간대별로 어떤 돌발에 대비해야 하는가. 도시고속국도는 4건 중 3건이 사고, 국가지원지방도는 5건 중 3건이 공사다. 전국 평균만 보고 대비하면 도시고속국도에서는 대응 자원의 52.5%p가 어긋난다.

</td>
</tr>
</table>

## 이렇게 판단합니다

| 원칙 | 실제로 한 일 |
|---|---|
| 결과를 보기 전에 기준을 정한다 | 대출·CRM 모두 가설 판정, 모델 선택, 운영 권고 규칙을 결과 확인 전에 고정하고 그대로 적용했다 |
| 복잡한 방법보다 단순한 방법과 먼저 비교한다 | CRM에서 "행동 있는 고객 우선" 단순 규칙만으로 포착률이 35%에서 64%로 오른다는 걸 먼저 확인하고, 모델이 그보다 나을 때만 모델을 권하도록 정했다 |
| 데이터가 이상하면 원인까지 확인한다 | 구매 기록 16%가 중복이었는데, 수량·시간 반올림·기록 오류 세 설명을 검증해 월초에 낮고 월말에 치솟는 패턴으로 원인을 좁혔다 |
| 결과가 좋을수록 의심한다 | CRM 결과가 지나치게 좋게 나오자 비교 기준이 약하게 잡혔는지 다시 검증했다. 대출에서는 너무 강한 신호에 미래 정보가 섞였는지 점검했다 |
| 틀린 가설도 그대로 쓴다 | "장바구니에서 뺀 고객은 덜 산다"는 가설이 정반대로 나왔다. 제거 고객의 34%가 24시간 안에 구매해, 리마인드 제외 대상이 아니라 우선 대상이라고 결론을 바꿨다 |

## 경험

- **국가연구개발과제 · e스포츠 시청 행태 분석(기업 연계)**: API로 장시간 수집 시 40분~1시간마다 수집이 끊기는 문제를 30분 단위 CSV 분할 저장 방식으로 바꿔 데이터 손실 없이 수집을 완료했습니다.
- **성균관대학교 수업조교(2024.03~2025.03, 약 50명 수업)**: 채점 공지 회차당 평균 문의 11건이 들어오던 것을, 채점·안내 기준을 통일한 뒤 4~5건으로 줄였습니다.

## 학력 · 자격

- 성균관대학교 스포츠과학과 석사(2025.08), 학사(2024.02)
- K-Digital Training 데이터 분석 수료(2025.12, 프로그래머스)
- SQLD · ADsP · GAIQ · OPIc IM1

## 연락처

dan980918@gmail.com
