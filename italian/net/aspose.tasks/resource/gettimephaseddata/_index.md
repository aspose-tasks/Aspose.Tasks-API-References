---
title: "Resource.GetTimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo di Resource. Restituisce un'istanza della classe TimephasedDataCollection per questo oggetto con i valori TimephasedData entro le date di inizio e fine specificate per il TimephasedDataType specificato"
type: docs
weight: 850
url: /it/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Restituisce un'istanza della classe [`TimephasedDataCollection`](../../timephaseddatacollection/) per questo oggetto con i valori [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate per il [`TimephasedDataType`](../../timephaseddatatype/).

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

Elenco di [`TimephasedData`](../timephaseddata/).

## Esempi

Mostra come leggere i dati timephased delle risorse di lavoro/costo.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Ottieni la Resource tramite il suo ID
var resource = project.Resources.GetByUid(1);

// Stampa i dati Timephased di ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Stampa i dati Timephased di ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Restituisce [`TimephasedDataCollection`](../../timephaseddatacollection/) per questo oggetto con i valori [`TimephasedData`](../timephaseddata/) entro le date di inizio e fine specificate.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | La data di inizio per i dati time phased. |
| fine | DateTime | La data di fine per i dati time phased. |

### Valore di ritorno

Elenco di [`TimephasedData`](../../timephaseddata/).

## Esempi

Mostra come leggere i dati timephased delle risorse di lavoro/costo.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Ottieni la Resource tramite il suo ID
var resource = project.Resources.GetByUid(1);

// Stampa i dati Timephased di ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Stampa i dati Timephased di ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


