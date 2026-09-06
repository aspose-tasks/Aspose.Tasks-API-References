---
title: "Tsk.IsResumeValid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否可以恢复"
type: docs
weight: 680
url: /zh/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

确定任务是否可以恢复。

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## 示例

展示如何读取/写入 Tsk.IsResumeValid 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


