---
title: "Tsk.IsActive"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否处于活动状态。非活动任务不再影响其他任务或整体项目进度表"
type: docs
weight: 550
url: /zh/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

确定任务是否处于活动状态。非活动任务不再影响其他任务或整体项目进度。

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## 示例

展示如何读取/写入 Tsk.IsActive 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


