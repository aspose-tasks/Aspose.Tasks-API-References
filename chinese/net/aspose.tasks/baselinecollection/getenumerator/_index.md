---
title: "BaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "BaselineCollection 方法。返回此集合的枚举器"
type: docs
weight: 50
url: /zh/net/aspose.tasks/baselinecollection/getenumerator/
---
## BaselineCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<Baseline> GetEnumerator()
```

### 返回值

此集合的枚举器。

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


