---
title: TaskLink.LinkLagTimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: TaskLink property. Gets or sets lag duration depending on LagFormat
type: docs
weight: 50
url: /net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Gets or sets lag duration, depending on LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | When trying to set the value for TaskLinks where LagFormat is TimeUnitType.Percent. |

## Remarks

Link lag can be a percentage value (LagFormat is TimeUnitType.Percent). In this case the duration is calculated as a percentage of PredTask's duration. Otherwise the method returns TimeSpan value representing TaskLink's lag.

### See Also

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


