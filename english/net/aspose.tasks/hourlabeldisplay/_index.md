---
title: Enum HourLabelDisplay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.HourLabelDisplay enum. Specifies how the hour label displays
type: docs
weight: 810
url: /net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Specifies how the hour label displays.

```csharp
public enum HourLabelDisplay
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| H | `0` | "h" label. |
| Hr | `1` | "hr" label. |
| Hour | `2` | "hour(s)" label. |

## Examples

Shows how to set the hour label of project's display options (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// set how the hour label is displayed
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


