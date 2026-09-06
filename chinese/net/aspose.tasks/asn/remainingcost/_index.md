---
title: "Asn.RemainingCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。完成任务的剩余预计成本"
type: docs
weight: 430
url: /zh/net/aspose.tasks/asn/remainingcost/
---
## Asn.RemainingCost field

完成分配的剩余预计成本。

```csharp
public static readonly Key<decimal, AsnKey> RemainingCost;
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


