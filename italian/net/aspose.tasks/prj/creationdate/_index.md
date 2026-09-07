---
title: "Prj.CreationDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data e l'ora in cui è stato creato un progetto"
type: docs
weight: 130
url: /it/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

La data e l'ora in cui è stato creato un progetto.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Osservazioni

Salvato in formato UTC nei file mpp. Tipo DateTime.

## Esempi

Mostra come leggere/scrivere la proprietà Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


