---
title: "Prj.NewTaskStartDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Тип даты начала по умолчанию для новых задач"
type: docs
weight: 580
url: /ru/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Тип даты начала по умолчанию для новых задач.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Примеры

Показывает, как задавать атрибуты для новых задач.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


