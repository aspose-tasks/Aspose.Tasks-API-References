---
title: "ResourceAssignment.MakeTPs"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment methode. Genereert een lijst met tijdgephaseerde gegevens"
type: docs
weight: 740
url: /nl/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Genereert een lijst met tijdgephaseerde gegevens.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | De opgegeven startdatum. |
| tijd | TimeSpan | De opgegeven werktijd. |
| kalender | Calendar | De opgegeven werkagenda. |
| lijst | List`1 | De lijst met tijdgephaseerde gegevens. |
| isWorking | Boolean | De opgegeven vlag die aangeeft of tijdgephaseerde gegevens werken of niet. |
| type | Int32 | Het opgegeven type tijdgephaseerde gegevens. |

### Retourwaarde

Een maximale datum uit de lijst of de startdatum als de lijst leeg is.

## Voorbeelden

Toont hoe TPs te genereren met parameters.

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

### Zie ook

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


