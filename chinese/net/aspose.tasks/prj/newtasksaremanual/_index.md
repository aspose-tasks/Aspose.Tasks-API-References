---
title: "Prj.NewTasksAreManual"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定新任务是否创建为手动"
type: docs
weight: 550
url: /zh/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

确定是否将新任务创建为手动。

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## 示例

展示如何读取/写入 Prj.NewTasksAreManual 属性。

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


