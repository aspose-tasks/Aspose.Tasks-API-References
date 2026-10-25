---
title: "Κλάση Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.Spreadsheet2003SaveOptions κλάση. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε Spreadsheet2003"
type: docs
weight: 2220
url: /el/net/aspose.tasks.saving/spreadsheet2003saveoptions/
---
## Spreadsheet2003SaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε Spreadsheet2003.

```csharp
public class Spreadsheet2003SaveOptions : SimpleSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Spreadsheet2003SaveOptions](spreadsheet2003saveoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `Spreadsheet2003SaveOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AssignmentView](../../aspose.tasks.saving/spreadsheet2003saveoptions/assignmentview/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής εργασιών για απόδοση ([`AssignmentViewColumn`](../../aspose.tasks.visualization/assignmentviewcolumn/)). |
| [ResourceView](../../aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής πόρων για απόδοση ([`ResourceViewColumn`](../../aspose.tasks.visualization/resourceviewcolumn/)). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |
| [View](../../aspose.tasks.saving/spreadsheet2003saveoptions/view/) { get; set; } | Λαμβάνει ή ορίζει μια λίστα των στηλών προβολής ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) για αποθήκευση. Εάν δεν οριστεί, τότε αποθηκεύονται οι προεπιλεγμένες στήλες. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες που θα εξαχθούν κατά την εξαγωγή του έργου σε μορφή Spreadsheet2003.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Δείτε επίσης

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


