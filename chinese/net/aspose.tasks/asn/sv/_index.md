---
title: "Asn.SV"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。项目状态日期截至的挣值进度偏差。进度偏差 SV 是 BCWP 与 BCWS 之间的差异"
type: docs
weight: 540
url: /zh/net/aspose.tasks/asn/sv/
---
## Asn.SV field

截至项目状态日期的挣值进度差异。进度差异（SV）是 BCWP 与 BCWS 之间的差额。

```csharp
public static readonly Key<double, AsnKey> SV;
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


