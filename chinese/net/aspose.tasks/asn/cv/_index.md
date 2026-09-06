---
title: "Asn.CV"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。已赚价值成本差异。CV 是分配的 BCWP（已完成工作预算成本）与 ACWP（实际完成工作成本）之间的差额"
type: docs
weight: 220
url: /zh/net/aspose.tasks/asn/cv/
---
## Asn.CV field

已获价值成本差异。CV 是任务的 BCWP（已完成工作预算成本）与 ACWP（实际完成工作成本）之间的差额。

```csharp
public static readonly Key<double, AsnKey> CV;
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


