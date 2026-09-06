---
title: "Asn.CostVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配的基线成本与总成本之间的差异"
type: docs
weight: 200
url: /zh/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

任务的基线成本与总成本之间的差额。

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## 示例

展示如何读取分配的差异。

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// 打印分配的差异
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


