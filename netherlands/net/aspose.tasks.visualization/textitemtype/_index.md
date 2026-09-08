---
title: "Enum TextItemType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.TextItemType enum. Itemtype om een tekststijl voor te wijzigen"
type: docs
weight: 3410
url: /nl/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Itemtype om een tekststijl voor te wijzigen.

```csharp
public enum TextItemType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| RowColumnTitles | `0` | Rij- en kolomtitels. |
| CriticalTasks | `1` | Kritieke taken. |
| NoncriticalTasks | `2` | Niet‑kritieke taken. |
| MilestoneTasks | `3` | Mijlpaaltaak. |
| InactiveTasks | `4` | Inactieve taken. |
| SummaryTasks | `5` | Samenvattingstaken. |
| AssignmentRow | `6` | Toewijzingsrij. |
| TopTimescaleTier | `7` | Bovenste tijdschaalniveau. |
| BottomTimescaleTier | `8` | Onderste tijdschaalniveau. |
| MiddleTimescaleTier | `9` | Middelste tijdschaalniveau. |
| Resources | `10` | Bronblad. |
| OverallocatedResources | `11` | Overgealloceerde resources. |
| TaskFilterHighlight | `12` | Taakfilter markering tekstitem. |
| BarTextBottom | `13` | Balktekst onderkant tekstitem. |
| BarTextInside | `14` | Balktekst binnen tekstitem. |
| BarTextLeft | `15` | Balktekst links tekstitem. |
| BarTextRight | `16` | Balktekst rechts tekstitem. |
| BarTextTop | `17` | Balktekst bovenkant tekstitem. |
| MarkedTasks | `18` | Gemarkeerde taak tekstitem. |
| ProjectSummary | `19` | Project samenvattingstaak tekstitem. |
| ExternalTasks | `20` | Externe taken tekstitem. |
| Allocated | `21` | Toegewezen tekstitem. |
| ChangedCells | `22` | Gewijzigde cellen. |

## Voorbeelden

Toont hoe te werken met tekstitemtypen.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


