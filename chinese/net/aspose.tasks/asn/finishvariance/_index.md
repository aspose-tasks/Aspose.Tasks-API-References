---
title: "Asn.FinishVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。任务完成日期相对于基准完成日期的偏差"
type: docs
weight: 250
url: /zh/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

任务完成日期相对于基线完成日期的偏差。

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


