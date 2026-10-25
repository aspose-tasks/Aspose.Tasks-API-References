---
title: "Tsk.IsPublished"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 确定当前任务是否应与项目的其余部分一起发布到 Project Server."
type: docs
weight: 660
url: /zh/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

确定当前任务是否应与项目的其他部分一起发布到 Project Server。

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## 示例

展示如何读取/写入 Tsk.IsPublished 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


