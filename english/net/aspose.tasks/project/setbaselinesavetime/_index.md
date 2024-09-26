---
title: Project.SetBaselineSaveTime
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Sets the baseline save time
type: docs
weight: 1260
url: /net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Sets the baseline save time.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | BaselineType | The baseline's number [`BaselineType`](../../baselinetype/). |
| value | DateTime | The baseline's last save date and time. |

## Remarks

Set value to DateTime.MinValue if the baseline was not saved.

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


