---
title: Enum BaselineType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BaselineType enum. Specifies the baseline type used to calculate Variance values
type: docs
weight: 130
url: /net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Specifies the baseline type used to calculate Variance values.

```csharp
public enum BaselineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates the field was not defined in original project file. |
| Baseline | `0` | Indicates Baseline type. |
| Baseline1 | `1` | Indicates Baseline1 type. |
| Baseline2 | `2` | Indicates Baseline2 type. |
| Baseline3 | `3` | Indicates Baseline3 type. |
| Baseline4 | `4` | Indicates Baseline4 type. |
| Baseline5 | `5` | Indicates Baseline5 type. |
| Baseline6 | `6` | Indicates Baseline6 type. |
| Baseline7 | `7` | Indicates Baseline7 type. |
| Baseline8 | `8` | Indicates Baseline8 type. |
| Baseline9 | `9` | Indicates Baseline9 type. |
| Baseline10 | `10` | Indicates Baseline10 type. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to set baseline for the project (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// save baseline fields to the specified baseline for the entire project.
project.SetBaseline(BaselineType.Baseline);
// work with project's baselines...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


