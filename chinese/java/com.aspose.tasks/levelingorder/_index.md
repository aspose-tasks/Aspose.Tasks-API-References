---
title: "LevelingOrder"
second_title: "Aspose.Tasks for Java API 参考"
description: "定义平衡顺序的可能取值。"
type: docs
weight: 143
url: /zh/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

定义平衡顺序的可能取值。
## 字段

| 字段 | 描述 |
| --- | --- |
| [IdOnly](#IdOnly) | 任务按 Id 升序延迟。 |
| [PriorityThenStandard](#PriorityThenStandard) | 首先考虑优先级，然后与 Standard 中相同的属性。 |
| [Standard](#Standard) | 以下属性将被考虑：前置关系、总松弛（总松弛更大的任务将首先被延迟）、开始日期、优先级。 |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


任务按 Id 升序延迟。

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


首先考虑优先级，然后与 Standard 中相同的属性。

### Standard {#Standard}
```
public static final int Standard
```


以下属性将被考虑：前置关系、总松弛（总松弛更大的任务将首先被延迟）、开始日期、优先级。这是默认值。

