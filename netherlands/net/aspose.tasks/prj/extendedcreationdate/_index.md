---
title: "Prj.ExtendedCreationDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. Datum gebruikt voor berekening en rapportage"
type: docs
weight: 320
url: /nl/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Datum gebruikt voor berekening en rapportage.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Voorbeelden

Toont hoe de eigenschap Prj.ExtendedCreationDate te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


