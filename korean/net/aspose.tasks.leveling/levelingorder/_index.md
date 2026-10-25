---
title: "열거형 LevelingOrder"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Leveling.LevelingOrder 열거형. 레벨링 순서의 가능한 값을 정의합니다."
type: docs
weight: 950
url: /ko/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

레벨링 순서의 가능한 값을 정의합니다.

```csharp
public enum LevelingOrder
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Standard | `1` | 다음 속성이 고려됩니다: 선행 관계, 총 여유시간(총 여유시간이 높은 작업이 먼저 지연됨), 시작 날짜, 우선순위. 이것이 기본값입니다. |
| IdOnly | `2` | 작업은 Id 오름차순으로 지연됩니다. |
| PriorityThenStandard | `3` | 우선순위가 먼저 고려되고, 그 다음에 Standard와 동일한 속성이 적용됩니다. |

### 또 보기

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


