---
title: "SplitPartCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SplitPartCollection 方法。返回此集合的枚举器"
type: docs
weight: 30
url: /zh/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### 返回值

此集合的枚举器。

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


