---
title: "Tsk.RegularWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La quantità totale di lavoro non straordinario programmato da eseguire dalle risorse"
type: docs
weight: 940
url: /it/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

La quantità totale di lavoro non straordinario programmato da eseguire dalle risorse.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


