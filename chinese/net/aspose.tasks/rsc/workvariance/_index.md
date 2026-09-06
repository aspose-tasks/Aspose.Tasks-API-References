---
title: "Rsc.WorkVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源基线工作与当前计划工作之间的差异"
type: docs
weight: 710
url: /zh/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

资源基线工作与当前计划工作之间的差异。

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## 示例

展示如何读取资源工作差异。

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


