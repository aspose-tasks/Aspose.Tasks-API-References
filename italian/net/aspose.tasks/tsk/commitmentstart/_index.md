---
title: "Tsk.CommitmentStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data di inizio di una consegna. Lettura supportata solo per il formato XML."
type: docs
weight: 180
url: /it/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

La data di inizio di una consegna. Lettura supportata solo per il formato XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


