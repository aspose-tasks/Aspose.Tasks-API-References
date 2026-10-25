---
title: "Prj.CustomDateFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Formato data personalizzato della vista progetto. Utilizzato per formattare le date quando la proprietà DateFormat è impostata su Custom"
type: docs
weight: 200
url: /it/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Formato data personalizzato della vista progetto. Utilizzato per formattare le date quando la proprietà [`DateFormat`](../dateformat/) è impostata su Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


