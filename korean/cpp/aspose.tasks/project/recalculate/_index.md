---
title: "Aspose::Tasks::Project::Recalculate 메서드"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "C++용 Aspose.Tasks"
description: "모든 프로젝트 작업의 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다."
type: docs
weight: 1130
url: /ko/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

모든 프로젝트 작업의 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

옵션 검증과 함께 모든 프로젝트 작업 ID, 개요 수준, 시작/완료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산합니다.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| 매개변수 | 설명 |
| --- | --- |
| 검증 | true이면 재계산 검증이 수행됩니다. 검증되는 데이터: 현재는 작업 및 작업 링크 날짜 범위에 대한 기본 검증만 구현되어 있습니다. 작업의 날짜 범위(예: ActualStart - ActualFinish, EarlyStart - EarlyFinish 등)와 작업 링크 날짜는 시작 날짜가 종료 날짜보다 작거나 같은지 확인하는 기준에 따라 검사됩니다. 위에 설명된 조건 중 하나라도 충족되지 않으면 RecalculationValidationException이 발생합니다. |

