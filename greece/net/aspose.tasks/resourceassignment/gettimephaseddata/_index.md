---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceAssignment. Επιστρέφει την παρουσία της κλάσης TimephasedDataCollection που περιέχει παρουσίες της κλάσης TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου TimephasedDataType."
type: docs
weight: 720
url: /el/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Επιστρέφει την παρουσία της κλάσης [`TimephasedDataCollection`](../../timephaseddatacollection/) που περιέχει παρουσίες της κλάσης [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| λήξη | DateTime | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |
| timephasedType | TimephasedDataType | Ο τύπος των δεδομένων χρονικής φάσης ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Τιμή Επιστροφής

επιστρέφει μια λίστα που περιέχει παρουσίες της κλάσης [`TimephasedData`](../../timephaseddata/).

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε δεδομένα χρονικής φάσης μιας ανάθεσης πόρων εντός ενός εύρους ημερομηνιών.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Ορίστε τις ιδιότητες του έργου
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Δημιουργήστε ανάθεση πόρων
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Ορίστε το περίγραμμα Backloaded, αυξάνει τη διάρκεια της εργασίας από 6 σε 10 ημέρες
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// λάβετε δεδομένα χρονικής φάσης
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Επιστρέφει το αντικείμενο [`TimephasedDataCollection`](../../timephaseddatacollection/) με τις παρουσίες της κλάσης [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης του AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| λήξη | DateTime | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |

### Τιμή Επιστροφής

επιστρέφει μια λίστα που περιέχει παρουσίες της κλάσης [`TimephasedData`](../../timephaseddata/).

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε δεδομένα χρονικής φάσης μιας ανάθεσης πόρων εντός ενός εύρους ημερομηνιών.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Ορίστε τις ιδιότητες του έργου
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Δημιουργήστε ανάθεση πόρων
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Ορίστε το περίγραμμα Backloaded, αυξάνει τη διάρκεια της εργασίας από 6 σε 10 ημέρες
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// λάβετε δεδομένα χρονικής φάσης
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


