---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceAssignment. Δημιουργεί λίστα δεδομένων χρονικά φάσεων βάσει της διάρκειας της εργασίας και της προγραμματισμένης ημερομηνίας έναρξης"
type: docs
weight: 780
url: /el/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

Δημιουργεί λίστα χρονοκαθορισμένων δεδομένων βάσει της διάρκειας της εργασίας και της προγραμματισμένης ημερομηνίας έναρξης.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ημερολόγιο | Calendar | Το ημερολόγιο από το οποίο θα δημιουργηθούν τα δεδομένα χρονικά φάσεων. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε μια διαίρεση για μια εργασία.

```csharp
var project = new Project();

// Αποκτήστε ένα τυπικό ημερολόγιο
var calendar = project.Get(Prj.Calendar);

// Ορίστε τις ρυθμίσεις ημερολογίου του έργου
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Προσθέστε μια νέα εργασία στην κύρια εργασία
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Δημιουργήστε μια νέα ανάθεση πόρων και δημιουργήστε δεδομένα χρονικά φάσεων
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Διαιρέστε την εργασία σε 3 μέρη.
// Παρέχετε τις παραμέτρους ημερομηνίας έναρξης και λήξης στη μέθοδο SplitTask που θα χρησιμοποιηθούν για τη διαίρεση.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


