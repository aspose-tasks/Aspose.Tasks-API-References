---
title: "Prj.StartDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De startdatum van een project"
type: docs
weight: 680
url: /nl/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

De startdatum van een project.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Voorbeelden

Toont hoe de eigenschap Prj.StartDate te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


