---
title: "Tsk.LevelingDelay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo di ritardo di un'attività rispetto alla sua data di inizio anticipata a causa del livellamento delle risorse"
type: docs
weight: 770
url: /it/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

Il tempo di ritardo di un'attività rispetto alla sua data di inizio anticipato a causa del livellamento delle risorse.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


