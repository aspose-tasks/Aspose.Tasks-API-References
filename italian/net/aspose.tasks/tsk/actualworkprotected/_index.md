---
title: "Tsk.ActualWorkProtected"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La durata durante la quale il lavoro effettivo è protetto. Lettura supportata solo per il formato XML"
type: docs
weight: 100
url: /it/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

La durata durante la quale il lavoro effettivo è protetto. Lettura supportata solo per il formato XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


