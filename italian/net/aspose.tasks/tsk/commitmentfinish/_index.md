---
title: "Tsk.CommitmentFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data di completamento di una consegna.  Lettura supportata solo per il formato XML"
type: docs
weight: 170
url: /it/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

La data di fine di una consegna. Lettura supportata solo per il formato XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


