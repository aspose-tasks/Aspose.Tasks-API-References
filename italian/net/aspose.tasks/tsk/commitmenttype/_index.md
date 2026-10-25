---
title: "Tsk.CommitmentType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività ha una consegna associata o una dipendenza da una consegna associata. Lettura supportata solo per il formato XML."
type: docs
weight: 190
url: /it/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Determina se un'attività ha una consegna associata o una dipendenza da una consegna associata. Lettura supportata solo per il formato XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


