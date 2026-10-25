---
title: "Prj.SplitsInProgressTasks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定进行中的任务是否可以拆分"
type: docs
weight: 650
url: /zh/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

确定进行中的任务是否可以拆分。

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## 示例

展示如何读取/写入 Prj.SplitsInProgressTasks 属性。

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


