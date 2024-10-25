---
title: LevelingOrder
second_title: Aspose.Tasks for Java API Reference
description: Defines the possible values of leveling order.
type: docs
weight: 142
url: /java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Defines the possible values of leveling order.
## Fields

| Field | Description |
| --- | --- |
| [IdOnly](#IdOnly) | Tasks are delayed in Id ascending order. |
| [PriorityThenStandard](#PriorityThenStandard) | The priority is considered first, then the same properties as in Standard. |
| [Standard](#Standard) | The following properties are taken into account: predecessor relationships, total slack (a task with higher total slack is delayed first), start date, priority. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Tasks are delayed in Id ascending order.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


The priority is considered first, then the same properties as in Standard.

### Standard {#Standard}
```
public static final int Standard
```


The following properties are taken into account: predecessor relationships, total slack (a task with higher total slack is delayed first), start date, priority. This is the default value.

