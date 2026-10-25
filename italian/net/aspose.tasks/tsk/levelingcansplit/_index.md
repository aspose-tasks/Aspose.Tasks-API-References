---
title: "Tsk.LevelingCanSplit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se la funzione di livellamento delle risorse può causare divisioni sul lavoro rimanente in questo compito"
type: docs
weight: 760
url: /it/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Determina se la funzione di livellamento delle risorse può causare suddivisioni del lavoro rimanente su questa attività.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


