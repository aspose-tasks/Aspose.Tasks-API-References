---
title: "ResourceAssignment.MakeTPs"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Genera un elenco di dati a intervalli temporali"
type: docs
weight: 740
url: /it/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Genera un elenco di dati a intervalli temporali.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | La data di inizio specificata. |
| tempo | TimeSpan | Il tempo di lavoro specificato. |
| calendario | Calendar | Il calendario di lavoro specificato. |
| elenco | List`1 | L'elenco dei dati a intervalli temporali. |
| isWorking | Boolean | Il flag specificato che indica se i dati a intervalli temporali sono operativi o meno. |
| tipo | Int32 | Il tipo di dati a intervalli temporali specificato. |

### Valore di ritorno

Una data massima dall'elenco o la data di inizio se l'elenco è vuoto.

## Esempi

Mostra come generare i TP tramite parametri.

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

### Vedi anche

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


