---
title: "Resource.GetTimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Resource. Επιστρέφει μια παρουσία της κλάσης TimephasedDataCollection για αυτό το αντικείμενο με τις τιμές TimephasedData εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου TimePhasedDataType"
type: docs
weight: 850
url: /el/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Επιστρέφει μια παρουσία της κλάσης [`TimephasedDataCollection`](../../timephaseddatacollection/) για αυτό το αντικείμενο με τις τιμές [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης του καθορισμένου [`TimephasedDataType`](../../timephaseddatatype/).

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

Λίστα των [`TimephasedData`](../timephaseddata/).

## Παραδείγματα

Δείχνει πώς να διαβάσετε δεδομένα χρονικής φάσης πόρων εργασίας/κόστους.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Αποκτήστε το Resource με το ID του
var resource = project.Resources.GetByUid(1);

// Εκτυπώστε τα δεδομένα χρονικής φάσης του ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Εκτυπώστε τα δεδομένα χρονικής φάσης του ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Επιστρέφει [`TimephasedDataCollection`](../../timephaseddatacollection/) για αυτό το αντικείμενο με τις τιμές [`TimephasedData`](../timephaseddata/) εντός των δοσμένων ημερομηνιών έναρξης και λήξης.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Η ημερομηνία έναρξης για τα δεδομένα χρονικής φάσης. |
| λήξη | DateTime | Η ημερομηνία λήξης για τα δεδομένα χρονικής φάσης. |

### Τιμή Επιστροφής

Λίστα των [`TimephasedData`](../../timephaseddata/).

## Παραδείγματα

Δείχνει πώς να διαβάσετε δεδομένα χρονικής φάσης πόρων εργασίας/κόστους.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Αποκτήστε το Resource με το ID του
var resource = project.Resources.GetByUid(1);

// Εκτυπώστε τα δεδομένα χρονικής φάσης του ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Εκτυπώστε τα δεδομένα χρονικής φάσης του ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


