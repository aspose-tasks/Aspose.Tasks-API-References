---
title: Enum MinuteLabelDisplay
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.MinuteLabelDisplay enum. Specifies how the minute label displays
type: docs
weight: 1020
url: /net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Specifies how the minute label displays.

```csharp
public enum MinuteLabelDisplay
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| M | `0` | Sets the Minutes list in MS Project as m. |
| Min | `1` | Sets the Minutes list in MS Project as min. |
| Minute | `2` | Sets the Minutes list in MS Project as minute. |

## Examples

Shows how to set the minute label of project's display options (case 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// set how the minute label is displayed
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


