---
title: "XlsxOptions.Encoding"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα XlsxOptions. Λαμβάνει ή ορίζει την κωδικοποίηση του τελικού αρχείου XLSX. Η προεπιλεγμένη τιμή είναι UTF8"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/xlsxoptions/encoding/
---
## XlsxOptions.Encoding property

Λαμβάνει ή ορίζει την κωδικοποίηση του τελικού αρχείου XLSX. Η προεπιλεγμένη τιμή είναι UTF8.

```csharp
public Encoding Encoding { get; set; }
```

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

* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


