---
title: "Classe TableTextStyle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.TableTextStyle. Rappresenta uno stile di testo in una tabella di visualizzazione"
type: docs
weight: 3370
url: /it/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Rappresenta uno stile di testo in una tabella di visualizzazione.

```csharp
public class TableTextStyle : TextStyle
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Inizializza una nuova istanza della classe `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Inizializza una nuova istanza della classe `TableTextStyle` con il font specificato. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Inizializza una nuova istanza della classe `TableTextStyle` con le impostazioni predefinite del font e lo stile del font specificato. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Inizializza una nuova istanza della classe `TableTextStyle` con la dimensione del font e lo stile del font specificati. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo dello stile di testo. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Ottiene o imposta il motivo di sfondo dello stile di testo. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Ottiene o imposta il colore del testo. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Ottiene o imposta un campo a cui applicare lo stile. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Ottiene o imposta il carattere dello stile del testo. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Restituisce un valore dell'enumerazione [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Ottiene un ID univoco della riga. Restituisce -1 se lo stile deve essere applicato a tutte le righe di una vista. |

## Esempi

Mostra come personalizzare gli stili di testo della tabella che sono usati per formattare diversi elementi di testo in un progetto.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// imposta lo stile di testo del nome del primo task
var style1 = new TableTextStyle(1);
// imposta un campo a cui applicare lo stile.
style1.Field = Field.TaskName;
// imposta <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> dello stile di testo.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// imposta la dimensione in punti del carattere dello stile di testo.

// imposta lo stile di testo della durata del secondo task
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // imposta un flag che indica che i dati della vista devono essere scritti
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Vedi anche

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


