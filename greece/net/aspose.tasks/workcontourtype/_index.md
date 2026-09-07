---
title: "Απαρίθμηση WorkContourType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WorkContourType απαρίθμηση. Καθορίζει το περίγραμμα μιας εργασίας"
type: docs
weight: 3610
url: /el/net/aspose.tasks/workcontourtype/
---
## WorkContourType enumeration

Καθορίζει το περίγραμμα μιας εργασίας.

```csharp
public enum WorkContourType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου. |
| Flat | `0` | Επίπεδο περίγραμμα εργασίας. |
| BackLoaded | `1` | Περίγραμμα εργασίας με φόρτωση στο τέλος. |
| FrontLoaded | `2` | Περίγραμμα εργασίας με φόρτωση στην αρχή. |
| DoublePeak | `3` | Περίγραμμα εργασίας διπλού κορυφής. |
| EarlyPeak | `4` | Περίγραμμα εργασίας πρώιμης κορυφής. |
| LatePeak | `5` | Περίγραμμα εργασίας καθυστερημένης κορυφής. |
| Bell | `6` | Περίγραμμα εργασίας τύπου καμπάνα. |
| Turtle | `7` | Περίγραμμα εργασίας τύπου χελώνας. |
| Contoured | `8` | Προσαρμοσμένο περίγραμμα εργασίας. |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να ορίσετε διαφορετικά περιγράμματα δεδομένων χρονικής φάσης για τις αναθέσεις πόρων.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 1, 3, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 1, 7, 17, 0, 0));

// προσθήκη εργασίας
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

var resource = project.Resources.Add("Resource");

// προσθήκη ανάθεσης πόρου
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(8));
resourceAssignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

// Το επίπεδο περίγραμμα είναι το προεπιλεγμένο περίγραμμα.
Console.WriteLine("Flat contour");

var collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("Turtle contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Turtle);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("BackLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.BackLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("FrontLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.FrontLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("Bell contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Bell);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("EarlyPeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.EarlyPeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("LatePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.LatePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Αλλαγή περιγράμματος.
Console.WriteLine("DoublePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.DoublePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


