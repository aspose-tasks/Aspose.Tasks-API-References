---
title: "TaskBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskBaselineCollection 属性。获取此 TaskBaselineCollection 对象中包含的对象数量。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

获取此 TaskBaselineCollection 对象中包含的对象数量。

```csharp
public int Count { get; }
```

## 示例

展示如何使用任务基线集合。

```csharp
var project = new Project();

// 创建项目基线
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 打印任务基线
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// 清除所有基线
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### 另见

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


