---
title: "Prj.WorkFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il formato usato per mostrare la durata dell'attività"
type: docs
weight: 790
url: /it/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Il formato utilizzato per mostrare la durata dell'attività.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Esempi

Mostra come ottenere una durata con il formato di lavoro predefinito.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// crea un valore di lavoro con il formato di lavoro predefinito del progetto
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


