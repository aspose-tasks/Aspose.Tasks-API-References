---
title: "Tsk.ConstraintDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。与约束类型关联的特定日期。"
type: docs
weight: 200
url: /zh/net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

与约束类型关联的特定日期。

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## 示例

展示如何获取/设置任务的约束。

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// 为 ID 为 11 的任务设置约束为尽可能晚。
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


