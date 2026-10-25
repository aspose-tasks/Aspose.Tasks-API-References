---
title: "Class TimephasedDataCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TimephasedDataCollection class. Vertegenwoordigt een verzameling van TimephasedData-objecten"
type: docs
weight: 2600
url: /nl/net/aspose.tasks/timephaseddatacollection/
---
## TimephasedDataCollection class

Vertegenwoordigt een verzameling van [`TimephasedData`](../timephaseddata/) objecten.

```csharp
public abstract class TimephasedDataCollection : IList<TimephasedData>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/timephaseddatacollection/count/) { get; } | Haalt het aantal objecten op dat in dit `TimephasedDataCollection`-object zit. |
| [IsReadOnly](../../aspose.tasks/timephaseddatacollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of de ICollection alleen-lezen is. |
| [Item](../../aspose.tasks/timephaseddatacollection/item/) { get; set; } | Retourneert het element op de opgegeven index. De set-accessor wordt niet ondersteund. eigenschap om tijdgephaseerde gegevens in te stellen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/timephaseddatacollection/add/)(TimephasedData) | Voegt een [`TimephasedData`](../timephaseddata/) instantie toe aan dit collectie‑object. |
| [AddRange](../../aspose.tasks/timephaseddatacollection/addrange/)(IEnumerable&lt;TimephasedData&gt;) | Voegt een verzameling van [`TimephasedData`](../timephaseddata/) instanties toe aan dit collectie‑object. |
| [Clear](../../aspose.tasks/timephaseddatacollection/clear/)() | Verwijdert alle items uit de `TimephasedDataCollection`. |
| [Contains](../../aspose.tasks/timephaseddatacollection/contains/)(TimephasedData) | Bepaalt of de `TimephasedDataCollection` een specifieke waarde bevat. |
| [CopyTo](../../aspose.tasks/timephaseddatacollection/copyto/)(TimephasedData[], int) | Kopieert de elementen van de `TimephasedDataCollection` naar een Array, beginnend bij een specifieke Array-index. |
| [GetEnumerator](../../aspose.tasks/timephaseddatacollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/timephaseddatacollection/remove/)(TimephasedData) | Verwijdert een [`TimephasedData`](../timephaseddata/) instantie uit dit collectie‑object. |
| [SelectBetweenStartAndFinish](../../aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/)(TimephasedDataType, DateTime, DateTime) | Selecteert alle tijdfasen tussen *startTime* en *finishTime*. Heeft een O(log n)-complexiteit in het gemiddelde geval. |
| [ToList](../../aspose.tasks/timephaseddatacollection/tolist/)() | Converteert het `TimephasedDataCollection`-object naar een lijst van [`TimephasedData`](../timephaseddata/) objecten. |

## Voorbeelden

Toont hoe te werken met tijdgephaseerde gegevensverzamelingen.

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

// stel contourwerkcontour in
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

Console.WriteLine("Is timephased data collection read-only?: " + assignment.TimephasedData.IsReadOnly);

// wis gegenereerde tds
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

// men kan de collectie filteren op type en datumbereik
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
// voeg een verkeerde td toe en verwijder deze vervolgens
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

// verwijder het verkeerde td-item
if (assignment.TimephasedData.Contains(td4))
{
    assignment.TimephasedData.Remove(td4);
}

// ...
assignment.TimephasedData.AddRange(list);

// itereren over tijdgephaseerde items
Console.WriteLine("Print all timephased items:");
Console.WriteLine("Timephased data count: " + assignment.TimephasedData.Count);
foreach (var item in assignment.TimephasedData)
{
    Console.WriteLine("Start: " + item.Start);
    Console.WriteLine("Finish: " + item.Finish);
    Console.WriteLine("Timephased Data Type: " + item.TimephasedDataType);
    Console.WriteLine();
}

// kopieer tds naar een andere toewijzing
var timephasedDatas = new TimephasedData[assignment.TimephasedData.Count];
assignment.TimephasedData.CopyTo(timephasedDatas, 0);

assignment2.TimephasedData.Clear();
foreach (var data in timephasedDatas)
{
    assignment2.TimephasedData.Add(data);
}

// de collectie kan worden omgezet naar een eenvoudige lijst
List<TimephasedData> tds = assignment.TimephasedData.ToList();

// laten we tds één voor één verwijderen
foreach (var timephasedData in tds)
{
    assignment.TimephasedData.Remove(timephasedData);
}
```

### Zie ook

* class [TimephasedData](../timephaseddata/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


