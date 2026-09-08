---
title: "Tsk.LevelingDelay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De tijd dat een taak moet worden vertraagd vanaf de vroegste startdatum vanwege resource leveling"
type: docs
weight: 770
url: /nl/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

De tijd waarmee een taak wordt vertraagd vanaf de vroegste startdatum vanwege resource-leveling.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.LevelingDelay te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


