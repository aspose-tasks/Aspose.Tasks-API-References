---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否将新资源或任务自动添加到资源或任务池"
type: docs
weight: 50
url: /zh/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

确定是否将新资源或任务自动添加到资源或任务池中。

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## 示例

展示如何读取/写入 Prj.AutoAddNewResourcesAndTasks 属性。

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


