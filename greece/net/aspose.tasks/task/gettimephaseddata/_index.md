---
title: "Task.GetTimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Επιστρέφει το αντικείμενο TimephasedDataCollection με τιμές TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου τύπου δεδομένων χρονικής φάσης"
type: docs
weight: 1360
url: /el/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Επιστρέφει το αντικείμενο [`TimephasedDataCollection`](../../timephaseddatacollection/) με τιμές [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου τύπου δεδομένων χρονικής φάσης.

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

Ένα αντικείμενο [`TimephasedDataCollection`](../../timephaseddatacollection/) με τιμές [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου τύπου δεδομένων χρονικής φάσης.

## Παραδείγματα

Δείχνει πώς να λάβετε δεδομένα χρονικής φάσης (με συγκεκριμένο τύπο) της εργασίας.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Επιστρέφει το αντικείμενο [`TimephasedDataCollection`](../../timephaseddatacollection/) με τιμές [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| λήξη | DateTime | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |

### Τιμή Επιστροφής

Λίστα των [`TimephasedData`](../../timephaseddata/) προς συμπλήρωση.

## Παραδείγματα

Δείχνει πώς να ληφθούν τα δεδομένα χρονικής φάσης (με τύπο TaskWork) της εργασίας.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


