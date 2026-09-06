---
title: "类 BaselineCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.BaselineCollection 类。表示 Baseline 对象的集合"
type: docs
weight: 120
url: /zh/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

表示 [`Baseline`](../baseline/) 对象的集合。

```csharp
public class BaselineCollection : IList<Baseline>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | 获取此 BaselineCollection 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | 获取此集合的父级 [`Resource`](../resource/)。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。 |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | 从此集合中移除基线。 |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | 将 BaselineCollection 对象转换为 [`Baseline`](../baseline/) 对象的列表。 |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


