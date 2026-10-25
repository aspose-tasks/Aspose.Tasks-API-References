---
title: "TableTextStyle.RowUid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TableTextStyle. Ottiene un ID univoco di riga. Restituisce 1 se lo stile deve essere applicato a tutte le righe di una vista"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/tabletextstyle/rowuid/
---
## TableTextStyle.RowUid property

Ottiene un ID univoco della riga. Restituisce -1 se lo stile deve essere applicato a tutte le righe di una vista.

```csharp
public int RowUid { get; }
```

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

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


