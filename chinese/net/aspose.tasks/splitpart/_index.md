---
title: "类 SplitPart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.SplitPart 类。表示任务的一部分。SplitPart 是任务 SplitParts 集合的成员。"
type: docs
weight: 2290
url: /zh/net/aspose.tasks/splitpart/
---
## SplitPart class

表示任务的一部分。SplitPart 是任务的 SplitParts 集合的成员。

```csharp
public class SplitPart
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | 获取 SplitPart 的结束日期。 |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | 获取 SplitPart 的开始日期。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | 比较两个拆分部分。 |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | 返回 `SplitPart` 类实例的哈希码值。 |

## 示例

展示如何处理已拆分任务的拆分部分。

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// 必须先生成资源分配的时间分段数据
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// 拆分任务。
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// 遍历拆分部分
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


