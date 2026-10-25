---
title: "LevelingDelayFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Il formato per esprimere la durata di un ritardo."
type: docs
weight: 790
url: /it/net/aspose.tasks/tsk/levelingdelayformat/
---
## Tsk.LevelingDelayFormat field

Il formato per esprimere la durata di un ritardo.

```csharp
public static readonly Key<TimeUnitType, TaskKey> LevelingDelayFormat;
```

### Esempi

Mostra come leggere/scrivere la proprietà Tsk.LevelingDelayFormat.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelayFormat, TimeUnitType.Hour);

Console.WriteLine("Leveling Delay Format: " + task.Get(Tsk.LevelingDelayFormat));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [TaskKey](../../taskkey)
* class [Tsk](../../tsk)
* namespace [Aspose.Tasks](../../tsk)
* assembly [Aspose.Tasks](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per Aspose.Tasks.dll -->
