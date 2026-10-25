---
title: "Asn.OvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。实际与剩余加班成本的总和"
type: docs
weight: 370
url: /zh/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

任务的实际加班成本与剩余加班成本之和。

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
```

## 示例

展示如何读取任务的加班/剩余工作/成本。

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// 打印任务的加班
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


