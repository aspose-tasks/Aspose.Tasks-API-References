---
title: "Rsc.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。所有任务已完成工作的百分比"
type: docs
weight: 550
url: /zh/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

所有任务已完成工作的百分比。

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## 示例

展示如何读取资源的工作完成百分比。

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// 显示所有资源的工作完成百分比
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


