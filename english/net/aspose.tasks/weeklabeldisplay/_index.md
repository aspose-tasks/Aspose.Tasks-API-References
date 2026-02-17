---
title: Enum WeekLabelDisplay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WeekLabelDisplay enum. Specifies how the week label displays
type: docs
weight: 3540
url: /net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Specifies how the week label displays.

```csharp
public enum WeekLabelDisplay
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| W | `0` | "w" label. |
| Wk | `1` | "wk" label. |
| Week | `2` | "week" label. |

## Examples

Shows how to set the week label of project's display options (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// set how the week label is displayed
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


