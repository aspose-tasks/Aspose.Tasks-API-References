---
title: Recalculate
second_title: .NET API 참조용 Aspose.Tasks
description: 모든 프로젝트 작업 ID 개요 수준 시작/종료 날짜 조기/지연 날짜 설정 여유 시간 작업 및 비용 필드를 계산합니다.
type: docs
weight: 1120
url: /ko/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜, 조기/지연 날짜 설정, 여유 시간, 작업 및 비용 필드를 계산합니다.

```csharp
public void Recalculate()
```

### 또한보십시오

* class [Project](../)
* 네임스페이스 [Aspose.Tasks](../../project/)
* 집회 [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

모든 프로젝트 작업 ID, 개요 수준, 시작/종료 날짜, 조기/지연 날짜 설정, 선택적 유효성 검사를 통해 슬랙, 작업 및 비용 필드를 다시 예약합니다.

```csharp
public void Recalculate(bool validate)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| validate | Boolean | true인 경우 재계산 유효성 검사가 수행됩니다. 유효성 검사되는 데이터: 현재 작업 및 작업 링크 날짜 범위의 기본 유효성 검사만 구현됩니다. 작업 날짜 범위(예: ActualStart - ActualFinish, EarlyStart - EarlyFinish 등) ) 뿐만 아니라 작업 링크 날짜는 시작 날짜가 완료 날짜보다 작거나 같은 날짜 기준에 대해 확인됩니다. 위에서 설명한 조건 중 하나라도 실패하면 다음[`RecalculationValidationException`](../../recalculationvalidationexception/)던질 것입니다. |

### 또한보십시오

* class [Project](../)
* 네임스페이스 [Aspose.Tasks](../../project/)
* 집회 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
