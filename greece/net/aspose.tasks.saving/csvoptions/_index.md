---
title: "Κλάση CsvOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.CsvOptions κλάση. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε CSV"
type: docs
weight: 1980
url: /el/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CsvOptions](csvoptions/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `CsvOptions` που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή CSV. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Λαμβάνει ή ορίζει μια κατηγορία δεδομένων προς αποθήκευση. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Λαμβάνει ή ορίζει μια κωδικοποίηση με την οποία θα αποθηκευτεί το CSV. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Λαμβάνει ή ορίζει ένα διαχωριστικό κειμένου. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, αποθηκεύονται οι προεπιλεγμένες στήλες. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; για να αποθηκεύσετε ένα έργο ως αρχείο CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


