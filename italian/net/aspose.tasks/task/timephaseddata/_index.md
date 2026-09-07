---
title: "Task.TimephasedData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene o imposta un oggetto TimephasedDataCollection di questo task. Il blocco di dati temporizzati associato a un task"
type: docs
weight: 1220
url: /it/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Ottiene o imposta un oggetto TimephasedDataCollection di questa attività. Il blocco di dati temporizzati associato a un'attività.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Osservazioni

Lettura supportata solo per il formato XML.

## Esempi

Mostra come iterare sui dati temporizzati del task.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
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


