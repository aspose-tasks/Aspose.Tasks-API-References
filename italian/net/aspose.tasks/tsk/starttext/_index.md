---
title: "Tsk.StartText"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Restituisce il testo di avvio dell'attività"
type: docs
weight: 1030
url: /it/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Restituisce il testo di avvio dell'attività.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


