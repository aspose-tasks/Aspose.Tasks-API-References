---
title: "Prj.StatusDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. la data di stato per visualizzare l'avanzamento o calcolare i totali del valore guadagnato. La data di stato è la stessa della data corrente, a meno che non venga specificata una data di stato diversa."
type: docs
weight: 690
url: /it/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

la data di stato per visualizzare l'avanzamento o per calcolare i totali del valore guadagnato. La data di stato è la stessa della data corrente (data di oggi) a meno che non venga specificata una data di stato diversa.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


