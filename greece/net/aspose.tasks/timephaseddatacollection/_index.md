---
title: "Κλάση TimephasedDataCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.TimephasedDataCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων TimephasedData"
type: docs
weight: 2600
url: /el/net/aspose.tasks/timephaseddatacollection/
---
## TimephasedDataCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`TimephasedData`](../timephaseddata/).

```csharp
public abstract class TimephasedDataCollection : IList<TimephasedData>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/timephaseddatacollection/count/) { get; } | Επιστρέφει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `TimephasedDataCollection`. |
| [IsReadOnly](../../aspose.tasks/timephaseddatacollection/isreadonly/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν το ICollection είναι μόνο για ανάγνωση. |
| [Item](../../aspose.tasks/timephaseddatacollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. Η πρόσβαση set δεν υποστηρίζεται. Ιδιότητα για ορισμό χρονικά φάσημα δεδομένων. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/timephaseddatacollection/add/)(TimephasedData) | Προσθέτει το στιγμιότυπο [`TimephasedData`](../timephaseddata/) σε αυτή τη συλλογή αντικειμένων. |
| [AddRange](../../aspose.tasks/timephaseddatacollection/addrange/)(IEnumerable&lt;TimephasedData&gt;) | Προσθέτει μια συλλογή από στιγμιότυπα [`TimephasedData`](../timephaseddata/) σε αυτή τη συλλογή αντικειμένων. |
| [Clear](../../aspose.tasks/timephaseddatacollection/clear/)() | Αφαιρεί όλα τα στοιχεία από το `TimephasedDataCollection`. |
| [Contains](../../aspose.tasks/timephaseddatacollection/contains/)(TimephasedData) | Καθορίζει εάν το `TimephasedDataCollection` περιέχει μια συγκεκριμένη τιμή. |
| [CopyTo](../../aspose.tasks/timephaseddatacollection/copyto/)(TimephasedData[], int) | Αντιγράφει τα στοιχεία του `TimephasedDataCollection` σε έναν Πίνακα, ξεκινώντας από έναν συγκεκριμένο δείκτη Πίνακα. |
| [GetEnumerator](../../aspose.tasks/timephaseddatacollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/timephaseddatacollection/remove/)(TimephasedData) | Αφαιρεί το στιγμιότυπο [`TimephasedData`](../timephaseddata/) από αυτή τη συλλογή αντικειμένων. |
| [SelectBetweenStartAndFinish](../../aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/)(TimephasedDataType, DateTime, DateTime) | Επιλέγει όλες τις χρονικές φάσεις μεταξύ *startTime* και *finishTime*. Έχει πολυπλοκότητα O(log n) σε μέση περίπτωση. |
| [ToList](../../aspose.tasks/timephaseddatacollection/tolist/)() | Μετατρέπει το αντικείμενο `TimephasedDataCollection` σε λίστα από αντικείμενα [`TimephasedData`](../timephaseddata/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές χρονικά φάσημα δεδομένων.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var resource2 = project.Resources.Add("Resource 2");
resource2.Set(Rsc.Type, ResourceType.Work);

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2019, 11, 11, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Work, project.GetDuration(3d, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

var assignment2 = project.ResourceAssignments.Add(task2, resource2);
assignment2.Set(Asn.Start, new DateTime(2019, 11, 11, 8, 0, 0));
assignment2.Set(Asn.Work, project.GetDuration(3, TimeUnitType.Hour));
assignment2.Set(Asn.Finish, new DateTime(2019, 11, 13, 17, 0, 0));

// ορίστε το περιγραμμικό περίγραμμα εργασίας
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// καθαρίστε τα παραγόμενα tds
assignment.TimephasedData.Clear();

var td = new TimephasedData
             {
                 Start = new DateTime(2019, 11, 11, 8, 0, 0),
                 Finish = new DateTime(2019, 11, 11, 9, 0, 0),
                 Uid = assignment.Get(Asn.Uid),
                 Unit = TimeUnitType.Hour,
                 Value = "PT1H0M0S",
                 TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
             };
assignment.TimephasedData.Add(td);

var list = new List<TimephasedData>();
var td2 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 12, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 12, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
var td3 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT1H0M0S",
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };

list.Add(td2);
list.Add(td3);
assignment.TimephasedData.AddRange(list);

// μπορείτε να φιλτράρετε τη συλλογή κατά τύπο και εύρος ημερομηνιών
Console.WriteLine("Print filtered tds:");
IList<TimephasedData> filteredTds = assignment.TimephasedData.SelectBetweenStartAndFinish(
    TimephasedDataType.AssignmentRemainingWork,
    new DateTime(2019, 11, 11, 0, 0, 0),
    new DateTime(2019, 11, 13));
foreach (var data in filteredTds)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("Timephased Data Type: " + data.TimephasedDataType);
    Console.WriteLine();
}

Console.WriteLine("--------------------------");
Console.WriteLine();

// ...
// προσθέστε ένα λανθασμένο td και στη συνέχεια διαγράψτε το
var td4 = new TimephasedData
              {
                  Start = new DateTime(2019, 11, 13, 8, 0, 0),
                  Finish = new DateTime(2019, 11, 13, 9, 0, 0),
                  Uid = assignment.Get(Asn.Uid),
                  Unit = TimeUnitType.Hour,
                  Value = "PT0H0M1S", // wrong value
                  TimephasedDataType = TimephasedDataType.AssignmentRemainingWork
              };
assignment.TimephasedData.Add(td4);

// ...

// διαγράψτε το λανθασμένο στοιχείο td
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// επανάληψη πάνω από στοιχεία timephased
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// αντιγράψτε τα tds σε άλλη ανάθεση
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// η συλλογή μπορεί να μετατραπεί σε απλή λίστα
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// ας αφαιρέσουμε τα tds ένα-ένα
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### Δείτε επίσης

* class [TimephasedData](../timephaseddata/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


