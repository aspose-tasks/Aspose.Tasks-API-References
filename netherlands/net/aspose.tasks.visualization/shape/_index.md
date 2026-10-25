---
title: "Enum Shape"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.Shape enum. Vorm van een marker aan het begin of einde van de balkstijl die wordt gerenderd bij het opslaan van weergavegegevens naar sommige SaveFileFormat."
type: docs
weight: 3360
url: /nl/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Vorm van een marker aan het begin of einde van de balkstijl die wordt gerenderd bij het opslaan van weergavegegevens naar sommige [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Geeft None-vorm aan. |
| VerticalLine | `1` | Geeft verticale lijnvorm aan. |
| Pentagon | `2` | Geeft pentagonvorm aan. |
| Triangle | `3` | Geeft driehoekvorm aan. |
| LeftBracket | `4` | Geeft linkerhaakvorm aan. |
| RightBracket | `5` | Geeft rechterhaakvorm aan. |
| ArrowDown | `6` | Geeft ArrowDown-vorm aan. |
| LeftFade | `7` | Geeft linkervervagingsvorm aan. |
| RightFade | `8` | Geeft rechtervervagingsvorm aan. |
| Diamond | `9` | Geeft diamantenvorm aan. |
| Circle | `10` | Geeft cirkelvorm aan. |

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


