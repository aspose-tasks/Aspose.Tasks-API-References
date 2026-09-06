---
title: "Task.SplitParts"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取一个 SplitPart 集合，表示任务的各个部分"
type: docs
weight: 1110
url: /zh/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

获取一个 SplitPart 集合，表示任务的各个部分。

```csharp
public SplitPartCollection SplitParts { get; }
```

## 示例

展示如何显示任务的拆分部分。

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// 访问任务
var task = project.RootTask.Children.GetById(4);

// 显示任务的拆分部分
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### 另见

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


