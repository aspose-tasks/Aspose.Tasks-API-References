---
title: "Gridline.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Gridline methode. Retourneert een vlag die aangeeft of dit exemplaar gelijk is aan het opgegeven object."
type: docs
weight: 50
url: /nl/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | het opgegeven object om te vergelijken met deze instantie. |

### Retourwaarde

een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object.

## Voorbeelden

Toont hoe de gelijkheid van rasterlijnen te controleren.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// De gelijkheid van rasterlijnen wordt gecontroleerd ten opzichte van het rasterlijntype.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// wijzig het type
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Zie ook

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


