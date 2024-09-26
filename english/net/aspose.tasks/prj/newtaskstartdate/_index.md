---
title: Prj.NewTaskStartDate
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The default start date type for new tasks
type: docs
weight: 580
url: /net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

The default start date type for new tasks.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Examples

Shows how to set attributes for new tasks.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


