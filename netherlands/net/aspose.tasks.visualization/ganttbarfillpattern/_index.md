---
title: "Enum GanttBarFillPattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern enum. Een vulpatroon voor vormen"
type: docs
weight: 3040
url: /nl/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Vulpatroon van een vorm.

```csharp
public enum GanttBarFillPattern
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Hollow | `0` | Hol patroon. |
| SolidFill | `1` | Solide vullingspatroon. |
| LightFill | `2` | Licht vullingspatroon. |
| MediumFill | `3` | Gemiddeld vullingspatroon. |
| DarkFill | `4` | Donker vullingspatroon. |
| DiagonalLeft | `5` | Diagonale linkspatroon (van linksboven naar rechtsonder). |
| DiagonalRight | `6` | Diagonale rechtspatroon (van rechtsboven naar linksonder). |
| DiagonalCross | `7` | Diagonale kruispatroon. |
| LineVertical | `8` | Lijn verticaal patroon. |
| LineHorizontal | `9` | Lijn horizontaal patroon. |
| LineCross | `10` | Lijn kruispatroon. |
| SolidFillWithDashedBorder | `11` | Solide met gestreepte rand patroon. |

## Voorbeelden

Toont hoe aangepaste balkstijlen van de Gantt-diagram projectweergave in te stellen.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Voeg de aangepaste balkstijl toe aan de collectie van aangepaste balken van de projectweergave.
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


