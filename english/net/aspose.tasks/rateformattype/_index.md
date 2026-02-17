---
title: Enum RateFormatType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RateFormatType enum. Specifies the units used by Microsoft Project to display a rate
type: docs
weight: 1620
url: /net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Specifies the units used by Microsoft Project to display a rate.

```csharp
public enum RateFormatType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | The value was not defined in original project file. |
| Minute | `0` | Minute ("min") |
| Hour | `1` | Hour ("hr") |
| Day | `2` | Day ("day") |
| Week | `3` | Week ("wk") |
| Month | `4` | Month ("mo") |
| Year | `5` | Year ("yr") |
| MaterialResourceRate | `6` | Material resource rate (empty) |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to read/write Rsc.StandardRateFormat property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


