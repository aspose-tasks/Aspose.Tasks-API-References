---
title: "Enumerazione TextItemType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enumerazione Aspose.Tasks.Visualization.TextItemType. Tipo di elemento per cambiare uno stile di testo."
type: docs
weight: 3410
url: /it/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Tipo di elemento per cui modificare uno stile di testo.

```csharp
public enum TextItemType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| RowColumnTitles | `0` | Titoli di riga e colonna. |
| CriticalTasks | `1` | Attività critiche. |
| NoncriticalTasks | `2` | Attività non critiche. |
| MilestoneTasks | `3` | Attività milestone. |
| InactiveTasks | `4` | Attività inattive. |
| SummaryTasks | `5` | Attività di riepilogo. |
| AssignmentRow | `6` | Riga di assegnazione. |
| TopTimescaleTier | `7` | Livello superiore della scala temporale. |
| BottomTimescaleTier | `8` | Livello inferiore della scala temporale. |
| MiddleTimescaleTier | `9` | Livello intermedio della scala temporale. |
| Resources | `10` | Foglio risorse. |
| OverallocatedResources | `11` | Risorse sovraassegnate. |
| TaskFilterHighlight | `12` | Elemento di testo Evidenzia filtro attività. |
| BarTextBottom | `13` | Elemento di testo Barra Inferiore. |
| BarTextInside | `14` | Elemento di testo Barra Interna. |
| BarTextLeft | `15` | Elemento di testo Barra Sinistra. |
| BarTextRight | `16` | Elemento di testo Barra Destra. |
| BarTextTop | `17` | Elemento di testo Barra Superiore. |
| MarkedTasks | `18` | Elemento di testo Attività contrassegnata. |
| ProjectSummary | `19` | Elemento di testo Attività riepilogo progetto. |
| ExternalTasks | `20` | Elemento di testo Attività esterne. |
| Allocated | `21` | Elemento di testo Allocato. |
| ChangedCells | `22` | Celle modificate. |

## Esempi

Mostra come lavorare con i tipi di elemento di testo.

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

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


