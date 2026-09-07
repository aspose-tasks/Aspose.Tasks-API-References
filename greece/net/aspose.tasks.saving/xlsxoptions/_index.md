---
title: "Κλάση XlsxOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Saving.XlsxOptions. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε XLSX"
type: docs
weight: 2270
url: /el/net/aspose.tasks.saving/xlsxoptions/
---
## XlsxOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε XLSX.

```csharp
public class XlsxOptions : SimpleSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [XlsxOptions](xlsxoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `XlsxOptions` που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή XLSX. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/xlsxoptions/assignmentview/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής εργασιών για απόδοση ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [Encoding](../../aspose.tasks.saving/xlsxoptions/encoding/) { get; set; } | Λαμβάνει ή ορίζει την κωδικοποίηση του τελικού αρχείου XLSX. Η προεπιλεγμένη τιμή είναι UTF8. |
| [ResourceView](../../aspose.tasks.saving/xlsxoptions/resourceview/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής πόρων για απόδοση ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |
| [View](../../aspose.tasks.saving/xlsxoptions/view/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) για αποθήκευση σε μορφή XLSX. Εάν δεν οριστεί, αποθηκεύονται οι προεπιλεγμένες στήλες. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο σε αρχείο XLSX χρησιμοποιώντας τις επιλογές &lt;see cref=\"P:Aspose.Tasks.Saving.XlsxOptions\"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Προσθέστε τις επιθυμητές στήλες του Gantt Chart
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Προσθέστε τις επιθυμητές στήλες προβολής πόρων
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Προσθέστε τις επιθυμητές στήλες προβολής ανάθεσης
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// ορίστε κωδικοποίηση
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Δείτε επίσης

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


