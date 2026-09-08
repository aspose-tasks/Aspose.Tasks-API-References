---
title: "Prj.TimescaleStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De datum waarop de tijdschaal in de weergave begint."
type: docs
weight: 740
url: /nl/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

De datum waarop de tijdschaal in de weergave begint.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Voorbeelden

Toont hoe de startdatum van de tijdschaal in te stellen om de datum te bepalen waarop de weergave moet beginnen.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


