---
title: "Enum LevelingOrder"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.Leveling.LevelingOrder enum. Definiert die möglichen Werte der Leveling-Reihenfolge"
type: docs
weight: 950
url: /de/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

Definiert die möglichen Werte der Leveling-Reihenfolge.

```csharp
public enum LevelingOrder
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Standard | `1` | Die folgenden Eigenschaften werden berücksichtigt: Vorgängerbeziehungen, Gesamtslack (eine Aufgabe mit höherem Gesamtslack wird zuerst verzögert), Startdatum, Priorität. Dies ist der Standardwert. |
| IdOnly | `2` | Aufgaben werden in aufsteigender Id-Reihenfolge verzögert. |
| PriorityThenStandard | `3` | Die Priorität wird zuerst berücksichtigt, dann die gleichen Eigenschaften wie im Standard. |

### Siehe auch

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


