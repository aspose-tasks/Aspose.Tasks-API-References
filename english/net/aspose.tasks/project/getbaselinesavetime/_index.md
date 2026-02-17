---
title: Project.GetBaselineSaveTime
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Returns the baseline save time
type: docs
weight: 1090
url: /net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Returns the baseline save time.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | BaselineType | The baseline's number [`BaselineType`](../../baselinetype/). |

### Return Value

The baseline's last save date and time.

## Remarks

Returns DateTime.MinValue if the baseline was not saved.

## Examples

Shows how to read/write project's baseline save time.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// set baseline save time
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### See Also

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


