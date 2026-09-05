---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API Reference"
description: "레벨링 순서의 가능한 값을 정의합니다."
type: docs
weight: 143
url: /ko/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

레벨링 순서의 가능한 값을 정의합니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [IdOnly](#IdOnly) | 작업은 Id 오름차순으로 지연됩니다. |
| [PriorityThenStandard](#PriorityThenStandard) | 우선 순위가 먼저 고려되고, 그 다음에 Standard와 동일한 속성이 적용됩니다. |
| [Standard](#Standard) | 다음 속성이 고려됩니다: 선행 관계, 총 여유시간(총 여유시간이 더 큰 작업이 먼저 지연됨), 시작 날짜, 우선 순위. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


작업은 Id 오름차순으로 지연됩니다.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


우선 순위가 먼저 고려되고, 그 다음에 Standard와 동일한 속성이 적용됩니다.

### Standard {#Standard}
```
public static final int Standard
```


다음 속성이 고려됩니다: 선행 관계, 총 여유시간(총 여유시간이 더 큰 작업이 먼저 지연됨), 시작 날짜, 우선 순위. 이것이 기본값입니다.

