---
title: "Tsk.FinishText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Restituisce il testo di fine del compito"
type: docs
weight: 410
url: /it/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Restituisce il testo di fine dell'attività.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


