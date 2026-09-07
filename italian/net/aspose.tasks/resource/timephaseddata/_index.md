---
title: "Resource.TimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene o imposta un'istanza della classe TimephasedDataCollection per questo oggetto"
type: docs
weight: 740
url: /it/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Ottiene o imposta un'istanza della classe [`TimephasedDataCollection`](../../timephaseddatacollection/) per questo oggetto.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Osservazioni

Lettura supportata solo per il formato XML.

## Esempi

Mostra come leggere i dati timephased della risorsa.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// itera sui dati timephased della risorsa
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Vedi anche

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


