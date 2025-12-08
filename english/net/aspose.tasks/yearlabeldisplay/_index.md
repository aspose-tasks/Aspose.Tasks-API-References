---
title: Enum YearLabelDisplay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.YearLabelDisplay enum. Specifies how the year label displays
type: docs
weight: 3630
url: /net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Specifies how the year label displays.

```csharp
public enum YearLabelDisplay
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Y | `0` | Sets the Years list in MS Project as mo. |
| Yr | `1` | Sets the Years list in MS Project as mon. |
| Year | `2` | Sets the Years list in MS Project as month. |

## Examples

Shows how to set the year label of project's display options (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// set how the year label is displayed
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


