---
title: "Tsk.DisplayOnTimeline"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Specifica se un'attività deve essere visualizzata in una vista timeline"
type: docs
weight: 290
url: /it/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Specifica se un'attività deve essere visualizzata nella vista a linea temporale.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


