---
title: "Prj.StatusDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. de statusdatum om voortgang weer te geven of om de totale verdiende waarde te berekenen. De statusdatum is dezelfde als de huidige datum, tenzij een andere statusdatum is opgegeven."
type: docs
weight: 690
url: /nl/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

de statusdatum om voortgang weer te geven of om de totale verdiende waarde te berekenen. De statusdatum is dezelfde als de huidige datum (de datum van vandaag) tenzij een andere statusdatum is opgegeven.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Voorbeelden

Toont hoe de eigenschap Prj.StatusDate te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


