---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceAssignment. Λαμβάνει την ποσότητα του timephased work για το καθορισμένο χρονικό διάστημα."
type: docs
weight: 730
url: /el/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Λαμβάνει το ποσό του χρονοκαθορισμένου έργου για το καθορισμένο χρονικό διάστημα.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Αρχή του χρονικού διαστήματος. |
| λήξη | DateTime | Τέλος του χρονικού διαστήματος. |
| timephasedDataType | TimephasedDataType | Τύπος των timephased δεδομένων προς χρήση. |

## Παραδείγματα

Δείχνει πώς να υπολογίσετε την εργασία της ανάθεσης για αυθαίρετο χρονικό διάστημα.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Εκτυπώστε την εργασία της ανάθεσης για κάθε ώρα.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Δείτε επίσης

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Λαμβάνει το ποσό του χρονοκαθορισμένου έργου για το καθορισμένο χρονικό διάστημα.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Αρχή του χρονικού διαστήματος. |
| λήξη | DateTime | Τέλος του χρονικού διαστήματος. |

### Δείτε επίσης

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


