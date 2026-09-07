---
title: "Prj.NewTaskStartDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il tipo di data di inizio predefinita per le nuove attività"
type: docs
weight: 580
url: /it/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Il tipo di data di inizio predefinita per le nuove attività.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Esempi

Mostra come impostare gli attributi per i nuovi task.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


