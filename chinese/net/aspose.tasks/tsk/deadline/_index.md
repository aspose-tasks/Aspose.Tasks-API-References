---
title: "Tsk.Deadline"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。指示任务完成时间的目标日期"
type: docs
weight: 270
url: /zh/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

指示任务完成时间的目标日期。

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## 示例

展示如何读取/写入 Tsk.Deadline 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


