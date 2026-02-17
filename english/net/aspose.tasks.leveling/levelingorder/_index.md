---
title: Enum LevelingOrder
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Leveling.LevelingOrder enum. Defines the possible values of leveling order
type: docs
weight: 940
url: /net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

Defines the possible values of leveling order.

```csharp
public enum LevelingOrder
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Standard | `1` | The following properties are taken into account: predecessor relationships, total slack (a task with higher total slack is delayed first), start date, priority. This is the default value. |
| IdOnly | `2` | Tasks are delayed in Id ascending order. |
| PriorityThenStandard | `3` | The priority is considered first, then the same properties as in Standard. |

### See Also

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


