---
title: "TableTextStyle.Field"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TableTextStyle. Λαμβάνει ή ορίζει ένα πεδίο στο οποίο θα εφαρμοστεί το στυλ. Field"
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/tabletextstyle/field/
---
## TableTextStyle.Field property

Λαμβάνει ή ορίζει ένα πεδίο στο οποίο θα εφαρμοστεί το στυλ. `Field`.

```csharp
public Field Field { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τα στυλ κειμένου πίνακα που χρησιμοποιούνται για τη μορφοποίηση διαφορετικών στοιχείων κειμένου σε ένα έργο.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// ορίστε το στυλ κειμένου του πρώτου ονόματος εργασίας
var style1 = new TableTextStyle(1);
// ορίστε ένα πεδίο στο οποίο θα εφαρμοστεί το στυλ.
style1.Field = Field.TaskName;
// ορίστε <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> του στυλ κειμένου.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// ορίστε το μέγεθος σε σημεία της γραμματοσειράς του στυλ κειμένου.

// ορίστε το στυλ κειμένου της διάρκειας της δεύτερης εργασίας
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // ορίστε μια σημαία που υποδεικνύει ότι τα δεδομένα προβολής πρέπει να γραφούν
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Δείτε επίσης

* enum [Field](../../../aspose.tasks/field/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


