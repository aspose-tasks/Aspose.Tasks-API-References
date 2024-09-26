---
title: Enum EarnedValueMethodType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.EarnedValueMethodType enum. Specifies the method used for calculating earned value
type: docs
weight: 480
url: /net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Specifies the method used for calculating earned value.

```csharp
public enum EarnedValueMethodType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | The field was not defined in original project file. |
| PercentComplete | `0` | Percent complete |
| PhysicalPercentComplete | `1` | Physical percent complete |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to specify the method used for calculating earned value (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// set earned value method type to 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// work with the project...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


