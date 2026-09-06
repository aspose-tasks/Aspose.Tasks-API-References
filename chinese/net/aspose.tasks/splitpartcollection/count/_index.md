---
title: "SplitPartCollection.Count"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SplitPartCollection 属性。获取集合中部分的数量"
type: docs
weight: 10
url: /zh/net/aspose.tasks/splitpartcollection/count/
---
## SplitPartCollection.Count property

获取集合中部分的数量。

```csharp
public int Count { get; }
```

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

* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


