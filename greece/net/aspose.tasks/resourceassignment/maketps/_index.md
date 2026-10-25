---
title: "ResourceAssignment.MakeTPs"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ResourceAssignment μέθοδος. Δημιουργεί μια λίστα δεδομένων χρονικής φάσης"
type: docs
weight: 740
url: /el/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Δημιουργεί μια λίστα χρονοκαθορισμένων δεδομένων.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Η καθορισμένη ημερομηνία έναρξης. |
| χρόνος | TimeSpan | Ο καθορισμένος χρόνος εργασίας. |
| ημερολόγιο | Calendar | Το καθορισμένο ημερολόγιο εργασίας. |
| λίστα | List`1 | Η λίστα των δεδομένων χρονικής φάσης. |
| isWorking | Boolean | Η καθορισμένη σημαία που υποδεικνύει εάν τα δεδομένα χρονικής φάσης είναι ενεργά ή όχι. |
| type | Int32 | Ο καθορισμένος τύπος δεδομένων χρονικής φάσης. |

### Τιμή Επιστροφής

Μέγιστη ημερομηνία από τη λίστα ή ημερομηνία έναρξης εάν η λίστα είναι κενή.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε TPs με παραμέτρους.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


