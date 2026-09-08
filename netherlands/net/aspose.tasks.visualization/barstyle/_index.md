---
title: "Klasse BarStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.BarStyle class. Wijzig de visuele stijl van de balk voor het item in de projectweergave"
type: docs
weight: 2960
url: /nl/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Wijzig de visuele stijl van de balk voor het item in de projectweergave.

```csharp
public class BarStyle
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [BarStyle](barstyle/)() | Initialiseert een nieuw exemplaar van de `BarStyle` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Krijgt of stelt Color van de balkstijl in. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Krijgt of stelt [`BarShape`](./barshape/) van de balkstijl in. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Geeft of stelt een door de gebruiker gedefinieerde converter in om tekst te renderen onder de balk van de taak. Overschrijft de waarde van de eigenschap [`BottomField`](./bottomfield/) . |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Krijgt of stelt een veld in dat onderaan de balk wordt weergegeven. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Krijgt of stelt [`Shape`](../shape/) aan het einde van de balk in. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Krijgt of stelt Color van de vorm aan het einde van de balk in. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Geeft of stelt een type van de eindvorm in. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Geeft of stelt een startpuntpositie van de gantt-balk in. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Geeft of stelt een door de gebruiker gedefinieerde converter in om tekst te renderen binnen de balk van de taak. Overschrijft de waarde van de eigenschap [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Krijgt of stelt een veld in dat binnen de balk wordt weergegeven. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Krijgt of stelt [`BarItemType`](../baritemtype/) van de balkstijl in. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Krijgt of stelt een door de gebruiker gedefinieerde converter in om tekst te verkrijgen die links van de taakbalk wordt weergegeven. Overschrijft de waarde van de [`LeftField`](./leftfield/) eigenschap. |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Krijgt of stelt een veld in dat links van de balk wordt weergegeven. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Geeft of stelt een door de gebruiker gedefinieerde converter in om tekst te renderen rechts van de balk van de taak. Overschrijft de waarde van de eigenschap [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Haalt een veld op of stelt het in dat rechts van de balk wordt weergegeven. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Haalt of stelt de [`Shape`](../shape/) aan het begin van de balk in. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Haalt of stelt de kleur van de vorm aan het begin van de balk in. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Geeft of stelt een type van de startvorm in. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Haalt of stelt de stijl van de tekst van de balk in. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Geeft of stelt een eindpuntpositie van de gantt-balk in. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Haalt op of stelt een door de gebruiker gedefinieerde converter in om tekst te verkrijgen die bovenaan de taakbalk wordt weergegeven. Overschrijft de waarde van de eigenschap [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Haalt een veld op of stelt het in dat bovenaan de balk wordt weergegeven. |

## Voorbeelden

Toont hoe aangepaste balkstijlen te gebruiken.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// voeg een balkstijl toe voor mijlpaaltaak.
var style = new BarStyle();
// stel <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> van de balkstijl in
style.ItemType = BarItemType.Milestone;
// stel <see cref="T:System.Drawing.Color" /> van de balkstijl in.
style.BarColor = Color.Green;
// stel <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> van de balkstijl in
style.BarShape = BarShape.HalfHeight;
// stel <see cref=\"T:Aspose.Tasks.Visualization.Shape\" /> in aan het begin van de balk
style.StartShape = Shape.LeftBracket;
// stel <see cref=\"T:System.Drawing.Color\" /> van de vorm in aan het begin van de balk
style.StartShapeColor = Color.Aqua;
// stel <see cref=\"T:Aspose.Tasks.Visualization.Shape\" /> in aan het einde van de balk
style.EndShape = Shape.RightBracket;
// stel <see cref=\"T:System.Drawing.Color\" /> van de vorm in aan het einde van de balk
style.EndShapeColor = Color.Aquamarine;
// stel de tekst in die rechts van de balk moet worden weergegeven.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// er bestaat een functie die het mogelijk maakt om de tekst van de balk te converteren
// laten we de converter instellen om de tekst voor de balk te verkrijgen die moet worden weergegeven.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// sla het project op
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


