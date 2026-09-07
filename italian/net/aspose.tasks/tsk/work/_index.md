---
title: "Tsk.Work"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo totale programmato su un'attività per tutte le risorse assegnate"
type: docs
weight: 1150
url: /it/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

Il tempo totale programmato su un'attività per tutte le risorse assegnate.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


