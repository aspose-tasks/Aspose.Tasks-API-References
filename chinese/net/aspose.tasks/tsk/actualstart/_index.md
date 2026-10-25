---
title: "Tsk.ActualStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务实际开始的日期和时间"
type: docs
weight: 80
url: /zh/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

任务实际开始的日期和时间。

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## 示例

展示在评估模式下项目的日期被重置。

```csharp
var project = new Project();

// 创建新任务
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


