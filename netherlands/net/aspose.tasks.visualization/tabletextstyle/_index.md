---
title: "Klasse TableTextStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.TableTextStyle klasse. Vertegenwoordigt een tekststijl in een weergavetabel"
type: docs
weight: 3370
url: /nl/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Stelt een tekststijl voor in een weergavetabel.

```csharp
public class TableTextStyle : TextStyle
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Initialiseert een nieuw exemplaar van de `TableTextStyle` klasse. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Initialiseert een nieuw exemplaar van de `TableTextStyle` klasse met het opgegeven lettertype. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Initialiseert een nieuw exemplaar van de `TableTextStyle` klasse met de standaard lettertype-instellingen en de opgegeven lettertype‑stijl. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Initialiseert een nieuw exemplaar van de `TableTextStyle` klasse met de opgegeven lettergrootte en lettertype‑stijl. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Haalt of stelt de achtergrondkleur van de tekststijl in. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Haalt of stelt het achtergrondpatroon van de tekststijl in. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Haalt op of stelt de kleur van de tekst in. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Haalt of stelt een veld in waarop de stijl moet worden toegepast. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Haalt op of stelt het lettertype van de tekststijl in. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Retourneert een waarde van de [`TextItemType`](../textitemtype/) enum. |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Haalt een unieke rij‑id op. Retourneer -1 als de stijl op alle rijen van een weergave moet worden toegepast. |

## Voorbeelden

Toont hoe tabeltekststijlen kunnen worden aangepast die worden gebruikt om verschillende tekstitems in een project te stijlen.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// stel eerste taaknaam tekststijl in
var style1 = new TableTextStyle(1);
// stel een veld in waarop de stijl moet worden toegepast.
style1.Field = Field.TaskName;
// stel <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> van de tekststijl in.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// stel grootte in punten van het lettertype van de tekststijl in.

// stel tweede taakduur tekststijl in
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // stel een vlag in die aangeeft dat weergavegegevens moeten worden geschreven
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Zie ook

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


