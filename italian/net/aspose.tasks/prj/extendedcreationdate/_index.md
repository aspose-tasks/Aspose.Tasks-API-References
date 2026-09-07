---
title: "Prj.ExtendedCreationDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Data usata per il calcolo e la reportistica"
type: docs
weight: 320
url: /it/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Data utilizzata per il calcolo e la reportistica.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


