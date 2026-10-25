---
title: "Klasse Gridline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.Gridline klasse. De horizontale of verticale lijn die verschijnt in de projectweergave"
type: docs
weight: 3100
url: /nl/net/aspose.tasks.visualization/gridline/
---
## Gridline class

De horizontale of verticale lijn die verschijnt in de projectweergave.

```csharp
public class Gridline
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Gridline](gridline/)() | Initialiseert een nieuw exemplaar van de `Gridline`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Haalt op of stelt de [`Color`](./color/) van een gridline in. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Haalt op of stelt het type van een gridline in ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Haalt op of stelt het [`LinePattern`](../linepattern/) van een gridline in. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Retourneert een hashcode-waarde voor het exemplaar van de `Gridline`-klasse. |

## Voorbeelden

Toont hoe te werken met rasterlijnen bij het opslaan in visuele formaten.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // stel het type van de rasterlijn in (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // stel de <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> van een rasterlijn in
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


