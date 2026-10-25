---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος FieldHelper. Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Επιστρέφει έναν προεπιλεγμένο τίτλο του συγκεκριμένου πεδίου.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| πεδίο | Πεδίο | Πεδίο για λήψη προεπιλεγμένου τίτλου. |

### Τιμή Επιστροφής

Προεπιλεγμένος τίτλος του συγκεκριμένου πεδίου εάν το πεδίο μπορεί να εμφανιστεί στην προβολή του MS Project, αλλιώς null.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


