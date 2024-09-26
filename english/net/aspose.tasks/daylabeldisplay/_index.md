---
title: Enum DayLabelDisplay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.DayLabelDisplay enum. Specifies how the day label displays
type: docs
weight: 440
url: /net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Specifies how the day label displays.

```csharp
public enum DayLabelDisplay
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| D | `0` | Sets the Days list in MS Project as d. |
| Dy | `1` | Sets the Days list in MS Project as dy. |
| Day | `2` | Sets the Days list in MS Project as day. |

## Examples

Shows how to set the day label of project's display options (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// set how the day label is displayed
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


