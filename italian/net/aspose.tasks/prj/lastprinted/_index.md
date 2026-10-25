---
title: "Prj.LastPrinted"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Ultimo orario di stampa del progetto. Salvato in formato UTC nei file mpp. Tipo DateTime"
type: docs
weight: 430
url: /it/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Ultimo orario di stampa del progetto. Salvato in formato UTC nei file mpp. Tipo DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


