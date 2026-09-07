---
title: "Task.GetTimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Restituisce un oggetto TimephasedDataCollection con valori TimephasedData entro le date di inizio e fine specificate per il tipo di dati timephased indicato."
type: docs
weight: 1360
url: /it/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Restituisce l'oggetto [`TimephasedDataCollection`](../../timephaseddatacollection/) con valori [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate per il tipo di dati time-phased.

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

Un oggetto [`TimephasedDataCollection`](../../timephaseddatacollection/) con valori [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate per il tipo di dati timephased.

## Esempi

Mostra come ottenere i dati timephased (con tipo specifico) dell'attività.

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

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Restituisce l'oggetto [`TimephasedDataCollection`](../../timephaseddatacollection/) con valori [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | La data di inizio per i dati time phased. |
| fine | DateTime | La data di fine per i dati time phased. |

### Valore di ritorno

Elenco di [`TimephasedData`](../../timephaseddata/) da compilare.

## Esempi

Mostra come ottenere i dati timephased (con tipo TaskWork) dell'attività.

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

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


