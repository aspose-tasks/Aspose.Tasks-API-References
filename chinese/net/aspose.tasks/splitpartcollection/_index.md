---
title: "类 SplitPartCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.SplitPartCollection 类。表示任务各部分的集合"
type: docs
weight: 2300
url: /zh/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

表示任务各部分的集合。

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | 获取集合中部分的数量。 |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | 检索任务在给定索引处的拆分部分。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | 将集合中的所有部分复制到新数组。 |

## 示例

展示如何使用拆分部分集合。

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// 遍历拆分部分
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// 按索引获取部分
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// 对任务的第一个拆分部分进行一些操作
```

### 另见

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


