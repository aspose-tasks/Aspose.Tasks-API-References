---
title: "Asn.ACWP"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。任务截至目前执行的工作实际成本。"
type: docs
weight: 90
url: /zh/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

截至目前分配上已完成工作的实际成本。

```csharp
public static readonly Key<double, AsnKey> ACWP;
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


