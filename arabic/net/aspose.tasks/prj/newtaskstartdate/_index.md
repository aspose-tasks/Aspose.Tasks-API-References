---
title: "Prj.NewTaskStartDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. نوع تاريخ البدء الافتراضي للمهام الجديدة"
type: docs
weight: 580
url: /ar/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

نوع تاريخ البدء الافتراضي للمهام الجديدة.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## الأمثلة

يوضح كيفية تعيين الخصائص للمهام الجديدة.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


