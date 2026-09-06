---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定在编辑链接时是否必须更新手动安排的任务"
type: docs
weight: 770
url: /zh/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

确定在链接被编辑时是否必须更新手动任务。

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## 示例

展示如何读取/写入 Prj.UpdateManuallyScheduledTasksWhenEditingLinks 属性。

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


