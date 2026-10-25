---
title: "Class ResourceViewColumn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.ResourceViewColumn klasse. Projectenweergaveklasse gebruikt in ResourceUsage-weergave en ResourceSheet-weergave"
type: docs
weight: 3350
url: /nl/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Klasse van projectweergave gebruikt in de ResourceUsage‑weergave en ResourceSheet‑weergave.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Initialiseert een nieuw exemplaar van de `ResourceViewColumn` klasse. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Initialiseert een nieuw exemplaar van de `ResourceViewColumn` klasse. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Initialiseert een nieuw exemplaar van de `ResourceViewColumn` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Kolomveld. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Haalt de kolomnaam op. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Haalt de uitlijning van de tekst op of stelt deze in (kan een van de waarden van de enumeratie [`HorizontalStringAlignment`](../horizontalstringalignment/) zijn). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Haalt de callback op of stelt deze in die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Haalt de kolombreedte op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Converteert de huidige resource naar de kolomtekst. |

## Voorbeelden

Toont hoe resource-weergavekolommen toe te voegen die geëxporteerd moeten worden.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// itereren over kolommen
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Zie ook

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


