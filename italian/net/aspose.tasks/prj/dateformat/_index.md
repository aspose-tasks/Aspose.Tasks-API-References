---
title: "Prj.DateFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Formato data della vista progetto"
type: docs
weight: 210
url: /it/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Formato data della vista progetto.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.DateFormat.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


