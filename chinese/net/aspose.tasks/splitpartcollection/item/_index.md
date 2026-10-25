---
title: "SplitPartCollection.Item"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SplitPartCollection 属性。检索在给定索引处的任务拆分部分"
type: docs
weight: 20
url: /zh/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

检索任务在给定索引处的拆分部分。

```csharp
public SplitPart this[int index] { get; set; }
```

| 参数 | 描述 |
| --- | --- |
| index | 部分索引。 |

### 返回值

一个拆分部分。

## 备注

索引从零开始。如果索引超出数组边界，则返回 null。

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


