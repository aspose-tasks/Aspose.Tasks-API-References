---
title: "Prj.TimescaleFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De datum waarop de tijdschaal in de weergave eindigt."
type: docs
weight: 730
url: /nl/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

De datum waarop de tijdschaal in de weergave eindigt.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Voorbeelden

Toont hoe de eigenschap Prj.TimescaleFinish te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


