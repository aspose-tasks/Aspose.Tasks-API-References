---
title: "Resource.Baselines"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取此对象的 BaselineCollection 实例。资源的基线值"
type: docs
weight: 160
url: /zh/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

获取此对象的 BaselineCollection 实例。资源的基线值。

```csharp
public BaselineCollection Baselines { get; }
```

## 示例

展示如何读取资源的基线。

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### 另见

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


