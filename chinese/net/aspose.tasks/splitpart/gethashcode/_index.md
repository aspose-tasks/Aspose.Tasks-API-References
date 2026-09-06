---
title: "SplitPart.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SplitPart 方法。返回 SplitPart 类实例的哈希码值。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

返回 [`SplitPart`](../) 类实例的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取拆分部件的哈希码。

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

// 拆分部件的相等性是根据起始、结束和索引进行检查的。
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// 基于拆分部件的起始、结束和索引的哈希码。 
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### 另见

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


