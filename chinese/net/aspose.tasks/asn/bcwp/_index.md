---
title: "Asn.BCWP"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。截至目前任务中已完成工作的预算成本"
type: docs
weight: 120
url: /zh/net/aspose.tasks/asn/bcwp/
---
## Asn.BCWP field

截至目前，已在任务上执行的工作的预算成本。

```csharp
public static readonly Key<double, AsnKey> BCWP;
```

## 示例

展示如何读取任务的成本值。

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// 打印资源任务成本
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


