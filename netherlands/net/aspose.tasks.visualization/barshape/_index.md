---
title: "Enum BarShape"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.BarShape enum. Vorm van een balkrechthoek"
type: docs
weight: 2950
url: /nl/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

Vorm van een balkrechthoek.

```csharp
public enum BarShape
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Full | `0` | Geeft volledige rechthoekige balkvorm aan. |
| HalfHeight | `1` | Geeft boven uitgelijnde halve hoogte rechthoekige balkvorm aan. |
| HalfHeightBottom | `2` | Geeft onder uitgelijnde halve hoogte rechthoekige balkvorm aan. |
| Thin | `3` | Geeft centraal uitgelijnde lijngvorm aan. |
| None | `4` | Geeft geen balkvorm aan. |
| Middle | `5` | Geeft centraal uitgelijnde lijngvorm aan. |
| LineBottom | `6` | Geeft onder uitgelijnde lijngvorm aan. |
| LineTop | `7` | Geeft boven uitgelijnde lijngvorm aan. |

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


