---
title: "ResourceAssignment.TimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ResourceAssignment. Λαμβάνει ή ορίζει την παρουσία της κλάσης TimephasedDataCollection που περιέχει στοιχεία της κλάσης TimephasedData"
type: docs
weight: 600
url: /el/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Λαμβάνει ή ορίζει την παρουσία της κλάσης [`TimephasedDataCollection`](../../timephaseddatacollection/) που περιέχει στοιχεία της κλάσης `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε δεδομένα timephased μιας ανάθεσης πόρων.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
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
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// λάβετε δεδομένα χρονικής φάσης
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


