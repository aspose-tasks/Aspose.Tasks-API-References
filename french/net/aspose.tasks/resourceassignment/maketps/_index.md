---
title: "ResourceAssignment.MakeTPs"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ResourceAssignment méthode. Génère une liste de données à phases temporelles"
type: docs
weight: 740
url: /fr/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Génère une liste de données phasées dans le temps.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date de début spécifiée. |
| temps | TimeSpan | Le temps de travail spécifié. |
| calendrier | Calendar | Le calendrier de travail spécifié. |
| liste | List`1 | La liste des données à phases temporelles. |
| isWorking | Boolean | Le drapeau spécifié qui indique si les données à phases temporelles sont actives ou non. |
| type | Int32 | Le type de données à phases temporelles spécifié. |

### Valeur de retour

Une date maximale provenant de la liste ou la date de début si la liste est vide.

## Exemples

Montre comment générer des TP par paramètres.

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

### Voir aussi

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


