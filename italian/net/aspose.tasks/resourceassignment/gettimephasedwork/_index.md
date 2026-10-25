---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ResourceAssignment metodo. Ottiene la quantità di lavoro timephased per l'intervallo di data e ora specificato"
type: docs
weight: 730
url: /it/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Ottiene la quantità di lavoro a intervalli temporali per l'intervallo di data/ora specificato.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | Inizio dell'intervallo di data e ora. |
| fine | DateTime | Fine dell'intervallo di data e ora. |
| timephasedDataType | TimephasedDataType | Tipo di dati timephased da utilizzare. |

## Esempi

Mostra come calcolare il lavoro dell'assegnazione per un intervallo di data e ora arbitrario.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Stampa il lavoro dell'assegnazione per ogni ora.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Vedi anche

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Ottiene la quantità di lavoro a intervalli temporali per l'intervallo di data/ora specificato.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | Inizio dell'intervallo di data e ora. |
| fine | DateTime | Fine dell'intervallo di data e ora. |

### Vedi anche

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


