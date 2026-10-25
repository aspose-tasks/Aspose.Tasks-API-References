---
title: "Enum GridlineType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.GridlineType enum. Type van rasterlijn."
type: docs
weight: 3110
url: /nl/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Type rasterlijn.

```csharp
public enum GridlineType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| GanttRow | `0` | Geeft rasterlijn van een Gantt‑rijtype aan. |
| TopTierColumn | `1` | Geeft rasterlijn van kolomtype bovenste laag aan. |
| BottomTierColumn | `2` | Geeft rasterlijn van kolomtype onderste laag aan. |
| SheetRow | `3` | Geeft rasterlijn van een blad‑rijtype aan. |
| SheetColumn | `4` | Geeft rasterlijn van een blad‑kolomtype aan. |
| UsageRow | `5` | Geeft rasterlijn van een gebruiks‑rijtype aan. |
| UsageColumn | `6` | Geeft rasterlijn van een gebruiks‑kolomtype aan. |
| GanttTitleVertical | `7` | Geeft verticale rasterlijn van de Gantt‑titel aan. |
| GanttTitleHorizontal | `8` | Geeft horizontale rasterlijn van de Gantt‑titel aan. |
| BarRows | `9` | Geeft rasterlijn van balkrijen aan. |
| GanttProjectStart | `10` | Geeft rasterlijn van Gantt‑projectstart aan. |
| GanttProjectFinish | `11` | Geeft rasterlijn van Gantt‑projecteinde aan. |
| GanttStatusDate | `12` | Geeft het rasterlijntype van de Gantt-statusdatum aan. |
| GanttCurrentDate | `13` | Geeft het rasterlijntype van de huidige Gantt-datum aan. |
| GanttPageBreaks | `14` | Geeft het rasterlijntype van Gantt-pagina-eindes aan. |
| MiddleTierColumn | `15` | Geeft het rasterlijntype van de middelste kolom aan. |

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


