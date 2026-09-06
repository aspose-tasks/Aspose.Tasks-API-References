---
title: "Asn.Resume"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Asn 字段。分配恢复的日期"
type: docs
weight: 490
url: /zh/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

分配恢复的日期。

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## 示例

展示如何读取分配的停止/恢复日期。

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// 打印资源分配的停止和恢复日期
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


