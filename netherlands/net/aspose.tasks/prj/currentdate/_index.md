---
title: "Prj.CurrentDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De systeemdatum"
type: docs
weight: 190
url: /nl/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

De systeemdatum.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Voorbeelden

Toont hoe de eigenschap Prj.CurrentDate te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


