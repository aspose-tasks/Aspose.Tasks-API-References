---
title: "BaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "BaselineCollection 方法。将 BaselineCollection 对象转换为 Baseline 对象的列表"
type: docs
weight: 70
url: /zh/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

将 BaselineCollection 对象转换为 [`Baseline`](../../baseline/) 对象的列表。

```csharp
public List<Baseline> ToList()
```

### 返回值

[`Baseline`](../../baseline/) 对象的列表。

## 示例

展示如何使用基线集合。

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// 读取基线信息
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### 另见

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


