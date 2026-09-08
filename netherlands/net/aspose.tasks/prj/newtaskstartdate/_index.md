---
title: "Prj.NewTaskStartDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het standaard startdatetype voor nieuwe taken"
type: docs
weight: 580
url: /nl/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Het standaard type startdatum voor nieuwe taken.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Voorbeelden

Toont hoe attributen voor nieuwe taken ingesteld worden.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


