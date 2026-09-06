---
title: "Asn.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配上已完成工作的量"
type: docs
weight: 400
url: /zh/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

在分配上已完成的工作量。

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## 示例

展示如何读取分配的工作完成百分比。

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// 打印分配的工作完成百分比
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


