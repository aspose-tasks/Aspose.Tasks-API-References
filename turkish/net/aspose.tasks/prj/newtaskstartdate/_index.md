---
title: "Prj.NewTaskStartDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Yeni görevler için varsayılan başlangıç tarihi türü"
type: docs
weight: 580
url: /tr/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Yeni görevler için varsayılan başlangıç tarihi türü.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Örnekler

Yeni görevler için özniteliklerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


