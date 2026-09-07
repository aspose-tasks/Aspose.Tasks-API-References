---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceAssignment. Restituisce l'istanza della classe TimephasedDataCollection contenente istanze della classe TimephasedData entro le date di inizio e fine specificate del TimephasedDataType specificato"
type: docs
weight: 720
url: /it/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Restituisce l'istanza della classe [`TimephasedDataCollection`](../../timephaseddatacollection/) contenente istanze della classe [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate del [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | La data di inizio per i dati time phased. |
| fine | DateTime | La data di fine per i dati time phased. |
| timephasedType | TimephasedDataType | Il tipo di dati time phased ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Valore di ritorno

restituisce un elenco che contiene istanze della classe [`TimephasedData`](../../timephaseddata/).

## Esempi

Mostra come generare dati timephased di un'assegnazione di risorsa entro un intervallo di date.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Imposta le proprietà del progetto
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Crea un'assegnazione di risorsa
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Imposta il contorno Backloaded, aumenta la durata dell'attività da 6 a 10 giorni
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// ottieni dati timephased
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Restituisce l'oggetto [`TimephasedDataCollection`](../../timephaseddatacollection/) con le istanze della classe [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate di AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | La data di inizio per i dati time phased. |
| fine | DateTime | La data di fine per i dati time phased. |

### Valore di ritorno

restituisce un elenco contenente istanze della classe [`TimephasedData`](../../timephaseddata/).

## Esempi

Mostra come generare dati timephased di un'assegnazione di risorsa entro un intervallo di date.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Imposta le proprietà del progetto
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Crea un'assegnazione di risorsa
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// Imposta il contorno Backloaded, aumenta la durata dell'attività da 6 a 10 giorni
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// ottieni dati timephased
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


