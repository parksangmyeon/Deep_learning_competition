\# Data Description



\## 데이터 개요



본 프로젝트는 고객의 금융 정보를 기반으로 `Credit\_Score`를 예측하는 다중분류 문제입니다.



데이터는 총 100,000개의 행과 28개의 컬럼으로 구성되어 있으며, 각 행은 고객의 월별 금융 상태를 나타냅니다.  

수치형 변수와 범주형 변수가 함께 포함된 표 형태의 정형 데이터입니다.



\## Target



| Column | Description |

|---|---|

| `Credit\_Score` | 예측 대상 변수로, 고객의 신용점수를 나타내는 다중분류 라벨입니다. |



\## 주요 입력 변수



| Column | Description |

|---|---|

| `Month` | 관측 월 |

| `Age` | 고객 나이 |

| `Occupation` | 고객 직업 |

| `Annual\_Income` | 연간 소득 |

| `Monthly\_Inhand\_Salary` | 월 실수령 급여 |

| `Num\_Bank\_Accounts` | 보유 은행 계좌 수 |

| `Num\_Credit\_Card` | 보유 신용카드 수 |

| `Interest\_Rate` | 적용 이자율 |

| `Num\_of\_Loan` | 보유 대출 수 |

| `Type\_of\_Loan` | 보유 대출 유형 |

| `Delay\_from\_due\_date` | 납부기한 이후 지연 일수 |

| `Num\_of\_Delayed\_Payment` | 지연 납부 횟수 |

| `Changed\_Credit\_Limit` | 신용 한도 변경 정도 |

| `Num\_Credit\_Inquiries` | 신용조회 횟수 |

| `Credit\_Mix` | 신용 구성 유형 |

| `Outstanding\_Debt` | 미상환 부채 |

| `Credit\_Utilization\_Ratio` | 신용 사용률 |

| `Credit\_History\_Age` | 신용 이력 기간 |

| `Payment\_of\_Min\_Amount` | 최소 금액 납부 여부 |

| `Total\_EMI\_per\_month` | 월별 총 EMI 상환액 |

| `Amount\_invested\_monthly` | 월별 투자 금액 |

| `Payment\_Behaviour` | 결제 행동 유형 |

| `Monthly\_Balance` | 월말 잔액 |



\## 제거한 변수



| Column | 제거 이유 |

|---|---|

| `ID` | 단순 식별자 변수로 예측에 직접적인 금융 정보를 제공하지 않는다고 판단했습니다. |

| `Customer\_ID` | 고객 식별자 변수로, 모델이 특정 고객을 외우는 누수 위험이 있다고 판단했습니다. |

| `Name` | 고객 이름으로 예측에 필요한 금융 정보가 아니라고 판단했습니다. |

| `SSN` | 개인 식별 정보로 예측 변수에서 제외했습니다. |



\## 데이터 특성



\- `Credit\_Score`는 3개 클래스로 구성된 다중분류 타겟입니다.

\- 클래스 비율 확인 결과 2번 클래스 비중이 가장 높고 0번 클래스 비중이 가장 낮았습니다.

\- 금액형 변수에서는 오른쪽으로 긴 꼬리 분포와 일부 극단값이 확인되었습니다.

\- `Type\_of\_Loan`은 여러 대출 유형이 하나의 문자열에 함께 포함된 복합 범주형 변수였습니다.

\- 실제 데이터 파일은 용량 및 라이선스 문제를 고려하여 GitHub에 포함하지 않았습니다.

