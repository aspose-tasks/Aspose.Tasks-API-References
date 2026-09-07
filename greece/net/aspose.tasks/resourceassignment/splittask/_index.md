---
title: "ResourceAssignment.SplitTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceAssignment. Διαχωρίζει την εργασία σε δύο μέρη"
type: docs
weight: 770
url: /el/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Διαιρεί την εργασία σε δύο μέρη.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Η αρχή της διακοπής εργασίας για τη διαίρεση. |
| τελείωση | DateTime | Το τέλος της διακοπής εργασίας για τη διαίρεση. |
| ημερολόγιο | Calendar | Το ημερολόγιο που θα χρησιμοποιηθεί για τη διαίρεση. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Ρίχνει εξαίρεση όταν η ημερομηνία έναρξης είναι μικρότερη από την ημερομηνία έναρξης της ανάθεσης. |
| ArgumentOutOfRangeException | Ρίχνει εξαίρεση όταν η ημερομηνία λήξης είναι μεγαλύτερη από την ημερομηνία λήξης της ανάθεσης. |

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


