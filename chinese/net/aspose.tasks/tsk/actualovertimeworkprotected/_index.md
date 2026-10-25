---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。实际加班工作受保护的持续时间"
type: docs
weight: 70
url: /zh/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

实际加班工作受到保护的持续时间。

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## 示例

展示如何读取/写入 Tsk.ActualOvertimeWorkProtected 属性。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


