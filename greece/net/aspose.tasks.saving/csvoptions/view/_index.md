---
title: "CsvOptions.View"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα CsvOptions. Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής GanttChartColumn για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες."
type: docs
weight: 60
url: /el/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες.

```csharp
public ProjectView View { get; set; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; για να πάρετε τις στήλες του προεπιλεγμένου Γράφηματος Gantt και

```csharp
// αποθηκεύστε τις σε αρχείο CSV.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### Δείτε επίσης

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


