---
title: "Duration.ToString"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Restituisce una rappresentazione stringa di questa istanza"
type: docs
weight: 120
url: /it/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Restituisce una rappresentazione stringa di questa istanza.

```csharp
public override string ToString()
```

### Valore di ritorno

una rappresentazione stringa di questa istanza.

## Esempi

Mostra come convertire una durata in una stringa.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// ottieni la durata dell'attività
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


