---
title: "Prj.DurationFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het formaat voor het weergeven van de totale duur"
type: docs
weight: 300
url: /nl/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Het formaat voor het uitdrukken van de totale duur.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Voorbeelden

Toont hoe de eigenschap Prj.DurationFormat te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


