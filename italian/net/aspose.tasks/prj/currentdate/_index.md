---
title: "Prj.CurrentDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data di sistema"
type: docs
weight: 190
url: /it/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

La data di sistema.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.CurrentDate.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


