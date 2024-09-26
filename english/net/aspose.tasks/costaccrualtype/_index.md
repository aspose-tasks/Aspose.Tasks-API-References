---
title: Enum CostAccrualType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CostAccrualType enum. Specifies the type of an accrual cost
type: docs
weight: 350
url: /net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

Specifies the type of an accrual cost.

```csharp
public enum CostAccrualType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates undefined value means that the field was not defined in original project file. |
| Start | `0` | Indicates Start cost accrual type. |
| Prorated | `1` | Indicates Prorated cost accrual type. |
| End | `2` | Indicates End cost accrual type. |
| Invalid | `3` | Indicates Invalid cost accrual type. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how and when resource standard and overtime costs are to be charged, or accrued (accrual method: Determines when the cost for a resource is incurred and when actual costs are charged to a project. You can incur costs at the start [Start] or finish [End] of a task or prorate them [Prorated] during the task.), to the cost of a task (CostAccrualType.End).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// set cost accrual type
// if you select the End option, costs are not accrued until remaining work is zero.
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// work with the project...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


