---
title: TaskLink.LinkLagTimeSpan
second_title: Aspose.Tasks för .NET API-referens
description: TaskLink fast egendom. Hämtar eller ställer in fördröjningslängd beroende på LagFormat.
type: docs
weight: 50
url: /sv/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Hämtar eller ställer in fördröjningslängd, beroende på LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | När du försöker ställa in värdet för TaskLinks där LagFormat är TimeUnitType.Percent. |

### Anmärkningar

Länkfördröjning kan vara ett procentuellt värde (LagFormat är TimeUnitType.Percent). I detta fall beräknas varaktigheten som en procentandel av PredTasks duration. Annars returnerar metoden TimeSpan-värde som representerar TaskLinks fördröjning.

### Se även

* class [TaskLink](../)
* namnutrymme [Aspose.Tasks](../../tasklink/)
* hopsättning [Aspose.Tasks](../../../)


