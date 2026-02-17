---
title: Enum MonthLabelDisplay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.MonthLabelDisplay enum. Specifies how the month label displays
type: docs
weight: 1050
url: /net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Specifies how the month label displays.

```csharp
public enum MonthLabelDisplay
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Mo | `0` | Sets the Months list in MS Project as mo. |
| Mon | `1` | Sets the Months list in MS Project as mon. |
| Month | `2` | Sets the Months list in MS Project as month. |

## Examples

Shows how to set the month label of project's display options (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// set how the month label is displayed
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


