---
title: "Prj.TaskUpdatesResource"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定任务的更新是否会更新资源"
type: docs
weight: 710
url: /zh/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

确定任务的更新是否会更新资源。

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## 示例

展示如何读取/写入 Prj.TaskUpdatesResource 属性。

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


