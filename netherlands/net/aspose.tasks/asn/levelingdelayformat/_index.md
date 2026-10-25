---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Het duurformaat van een vertraging."
type: docs
weight: 320
url: /nl/net/aspose.tasks/asn/levelingdelayformat/
---
## Asn.LevelingDelayFormat field

Het duurformaat van een vertraging.

```csharp
public static readonly Key<TimeUnitType, AsnKey> LevelingDelayFormat;
```

### Voorbeelden

Toont hoe de eigenschappen Asn.Delay, Asn.LevelingDelay en Asn.LevelingDelayFormat te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
Console.WriteLine("Leveling Delay Format: " + assignment.Get(Asn.LevelingDelayFormat));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
