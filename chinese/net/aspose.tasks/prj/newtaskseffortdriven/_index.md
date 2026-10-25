---
title: "Prj.NewTasksEffortDriven"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定新任务是否以工时为驱动"
type: docs
weight: 560
url: /zh/net/aspose.tasks/prj/newtaskseffortdriven/
---
## Prj.NewTasksEffortDriven field

确定新任务是否基于工作量驱动。

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEffortDriven;
```

## 示例

展示如何读取/写入 Prj.NewTasksEffortDriven 属性。

```csharp
var project = new Project();

project.Set(Prj.NewTasksEffortDriven, true);

Console.WriteLine("New Tasks Effort Driven: " + project.Get(Prj.NewTasksEffortDriven));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


