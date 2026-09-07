---
title: "Prj.StartDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data di inizio di un progetto"
type: docs
weight: 680
url: /it/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

La data di inizio di un progetto.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


