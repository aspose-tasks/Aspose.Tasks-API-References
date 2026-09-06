---
title: "Task.Baselines"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取或设置任务基线值的集合"
type: docs
weight: 130
url: /zh/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

获取或设置任务的基线值集合。

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## 示例

展示如何读取任务的基线。

```csharp
var project = new Project();

// 设置基线
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 显示任务基线持续时间
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### 另见

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


