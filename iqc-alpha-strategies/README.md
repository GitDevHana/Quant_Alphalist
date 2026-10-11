# WorldQuant BRAIN IQC — Alpha Research Archive

WorldQuant BRAIN IQC 관련 Alpha 후보 수식 16개를 정리한 아카이브입니다.

> **공개 전 확인:** 대회 규정, WorldQuant BRAIN 이용약관, 데이터/수식 공개 가능 여부 및 팀원 간 공유 권한을 먼저 확인해야 합니다. 확인 전에는 private 저장소 사용을 권장합니다.

## Overview

- **Format:** WorldQuant BRAIN Fast Expression 계열 수식(사용자 제공 원본)
- **Contents:** AP01–AP16, 각각 별도 텍스트 파일
- **Purpose:** 전략 아이디어 기록 및 비교를 위한 연구 아카이브
- **Verification:** 실행 성공, 플랫폼 지원 여부, 백테스트 지표 및 대회 제출·통과 여부는 확인되지 않았습니다.
- **Authorship:** 개별 Alpha의 최초 제안자/수정자 및 팀 기여도를 이 자료만으로 확인할 수 없습니다.

## Alpha List

| ID | Strategy theme (interpretive label) |
|---|---|
| [AP01](alphas/alpha_01.txt) | CLV + volume trend |
| [AP02](alphas/alpha_02.txt) | Positive return days with liquidity trigger |
| [AP03](alphas/alpha_03.txt) | CLV long and momentum short |
| [AP04](alphas/alpha_04.txt) | Positive days / fundamental ranking |
| [AP05](alphas/alpha_05.txt) | Short-horizon reversal with group neutralization |
| [AP06](alphas/alpha_06.txt) | Fundamental risk composite |
| [AP07](alphas/alpha_07.txt) | Analyst book-value estimate spread |
| [AP08](alphas/alpha_08.txt) | Return divergence and volatility |
| [AP09](alphas/alpha_09.txt) | Intraday price-band deviation |
| [AP10](alphas/alpha_10.txt) | CLV long and ROC short |
| [AP11](alphas/alpha_11.txt) | Operating-income long and ROC short |
| [AP12](alphas/alpha_12.txt) | EV/EBITDA and sentiment grouping |
| [AP13](alphas/alpha_13.txt) | Financial ratios and exchange grouping |
| [AP14](alphas/alpha_14.txt) | News signal and price reversal |
| [AP15](alphas/alpha_15.txt) | Reversal with group-mean neutralization |
| [AP16](alphas/alpha_16.txt) | EPS and sales estimate grouping |

## Notes

- 코드는 제공받은 수식을 그대로 옮겼으며, 문법이나 수학적 동작을 자동 수정하지 않았습니다.
- `AP04`는 여러 식이 연속되어 있어 플랫폼에서 최종 반환되는 표현식이 의도와 같은지 확인이 필요합니다.
- 일부 식은 `#` 주석, 데이터 필드 타입, 그룹 인자, 0으로 나누기 등의 문제로 플랫폼에서 조정이 필요할 수 있습니다.
- 수식에 사용된 필드 및 연산자는 WorldQuant BRAIN 환경에 종속되며, 일반 Python 코드가 아닙니다.
- 투자 성과 또는 실제 수익성을 보증하지 않습니다.

## Repository layout

```text
alphas/
  alpha_01.txt
  ...
  alpha_16.txt
README.md
```

## Portfolio description (optional)

WorldQuant BRAIN IQC 팀 프로젝트에서 Fast Expression 기반 Alpha 전략을 연구하고, 전략 테스트 과정의 반복 작업을 줄이기 위한 로컬 검증 도구 개발에 참여했습니다. 이 저장소는 연구 과정의 Alpha 후보 수식을 별도 정리한 자료이며, 공식 평가 성과를 의미하지 않습니다.
