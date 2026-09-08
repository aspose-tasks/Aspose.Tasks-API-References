---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Het formaat voor het uitdrukken van de duur van een vertraging."
type: docs
weight: 790
url: /nl/net/aspose.tasks/tsk/levelingdelayformat/
---
## Tsk.LevelingDelayFormat field

Het formaat voor het uitdrukken van de duur van een vertraging.

```csharp
public static readonly Key<TimeUnitType, TaskKey> LevelingDelayFormat;
```

### Voorbeelden

Toont hoe de eigenschap Tsk.LevelingDelayFormat te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelayFormat, TimeUnitType.Hour);

Console.WriteLine("Leveling Delay Format: " + task.Get(Tsk.LevelingDelayFormat));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [TaskKey](../../taskkey)
* class [Tsk](../../tsk)
* namespace [Aspose.Tasks](../../tsk)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
