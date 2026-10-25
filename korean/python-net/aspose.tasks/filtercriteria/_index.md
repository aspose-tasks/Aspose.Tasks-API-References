---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Python via .NET API 참조"
description: 
type: docs
weight: 350
url: /ko/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 정의합니다.

FilterCriteria 유형은 다음 멤버를 노출합니다:
## 생성자
| 이름 | 설명 |
| :- | :- |
| FilterCriteria() | FilterCriteria 클래스의 새 인스턴스를 초기화합니다 |
## 속성
| 이름 | 설명 |
| :- | :- |
| 작업 | FieldName, Test 및 Value와 함께 설정된 기준을 가져오거나 설정합니다. 이 기준은 필터의 다른 기준과 관련됩니다. |
| field | 변경할 [field](/tasks/python-net/aspose.tasks/filtercriteria/)을 가져오거나 설정합니다. |
| test | FieldName과 Value 사이에 수행되는 비교 유형을 가져오거나 설정합니다. 이 비교는 필터의 선택 기준으로 작동합니다.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | FieldName으로 지정된 필드의 값과 비교할 객체 값을 가져옵니다. |
| criteria_rows | 자식 [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) 행 목록을 가져옵니다.<br/>            필터에 둘 이상의 기준 행이 포함된 경우, And 연산자의 효과는 두 행의 기준이 모두 충족되어야 해당 작업 또는 리소스가 이 필터의 결과로 표시된다는 것입니다.<br/>            Or 연산자의 효과는 두 행 중 하나의 기준만 충족하면 된다는 것입니다. |
## 메서드
| 이름 | 설명 |
| :- | :- |
| is_field_value() | FilterCriteria의 오른쪽 값이 상수 값이 아니라 필드 참조인지 여부를 가져옵니다. |
| set_value_field(value) | FieldName으로 지정된 필드의 값과 비교될 필드의 값을 설정합니다. |

### 또 보기

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

