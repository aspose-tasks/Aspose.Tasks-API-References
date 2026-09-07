---
title: "Tsk.DurationText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Restituisce il testo della durata del compito"
type: docs
weight: 310
url: /it/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Restituisce il testo della durata dell'attività.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


