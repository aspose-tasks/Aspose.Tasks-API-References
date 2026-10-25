---
title: "Asn.StartVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配开始日期相对于基线开始日期的差异"
type: docs
weight: 510
url: /zh/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

分配开始日期相对于基线开始日期的偏差。

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


