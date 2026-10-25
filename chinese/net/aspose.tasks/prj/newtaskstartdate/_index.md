---
title: "Prj.NewTaskStartDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。新任务的默认开始日期类型"
type: docs
weight: 580
url: /zh/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

新任务的默认开始日期类型。

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## 示例

展示如何为新任务设置属性。

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


