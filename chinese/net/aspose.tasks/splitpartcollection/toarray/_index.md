---
title: "SplitPartCollection.ToArray"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SplitPartCollection 方法。将集合中的所有部分复制到新数组"
type: docs
weight: 40
url: /zh/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

将集合中的所有部分复制到新数组。

```csharp
public SplitPart[] ToArray()
```

### 返回值

一个包含 [`SplitPart`](../../splitpart/) 对象的数组。

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


